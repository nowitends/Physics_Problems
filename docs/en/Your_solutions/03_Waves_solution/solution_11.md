<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Young's Double-Slit Simulator</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body { background-color: #030712; color: #e5e7eb; overflow-x: hidden; }
        .glass { background: rgba(17, 24, 39, 0.7); backdrop-filter: blur(10px); border: 1px solid rgba(255,255,255,0.1); }
        input[type=range] { accent-color: #6366f1; cursor: ew-resize; }
        canvas { image-rendering: pixelated; }
    </style>
</head>
<body class="p-4 md:p-8 min-h-screen">

    <div class="max-w-6xl mx-auto space-y-6">
        <!-- Header -->
        <header class="flex justify-between items-end border-b border-slate-800 pb-4">
            <div>
                <h1 class="text-3xl font-black tracking-tighter text-white">YOUNG'S <span class="text-indigo-500">EXPERIMENT</span></h1>
                <p class="text-slate-500 text-xs font-mono uppercase tracking-widest">Two-Slit Coherent Interference</p>
            </div>
            <div class="text-right hidden md:block">
                <p class="text-[10px] font-mono text-slate-500">FORMULA: u = Σ (A/rᵢ) sin(krᵢ - ωt)</p>
            </div>
        </header>

        <div class="grid grid-cols-1 lg:grid-cols-12 gap-6">
            <!-- Controls Panel -->
            <div class="lg:col-span-3 space-y-6 glass p-6 rounded-3xl">
                <div>
                    <div class="flex justify-between mb-2">
                        <label class="text-[10px] font-bold text-slate-400 uppercase tracking-widest">Slit Distance (d)</label>
                        <span id="dVal" class="text-indigo-400 font-mono text-xs">50 px</span>
                    </div>
                    <input type="range" id="dSlider" min="10" max="150" step="1" value="50" class="w-full h-2 bg-slate-800 rounded-lg appearance-none">
                </div>

                <div>
                    <div class="flex justify-between mb-2">
                        <label class="text-[10px] font-bold text-slate-400 uppercase tracking-widest">Wavelength (λ)</label>
                        <span id="lVal" class="text-emerald-400 font-mono text-xs">40 px</span>
                    </div>
                    <input type="range" id="lSlider" min="10" max="100" step="1" value="40" class="w-full h-2 bg-slate-800 rounded-lg appearance-none">
                </div>

                <div class="pt-4 border-t border-slate-800 space-y-4">
                    <div class="bg-indigo-950/30 p-4 rounded-2xl border border-indigo-500/20">
                        <h3 class="text-xs font-bold text-indigo-300 mb-2 uppercase">Observation:</h3>
                        <p class="text-[11px] text-slate-400 leading-relaxed italic">
                            Increase <span class="text-white">d</span> to see more interference fringes. Increase <span class="text-white">λ</span> to see the fringes spread apart.
                        </p>
                    </div>
                    <button id="resetTime" class="w-full py-2 bg-slate-800 hover:bg-slate-700 text-slate-300 rounded-xl text-xs font-bold transition-all uppercase tracking-widest">
                        Sync Phase
                    </button>
                </div>
            </div>

            <!-- Main Canvas Viewport -->
            <div class="lg:col-span-9 relative group">
                <div class="absolute top-4 left-6 z-10 pointer-events-none">
                    <span class="bg-black/50 backdrop-blur px-3 py-1 rounded-full text-[10px] font-bold text-white uppercase tracking-widest border border-white/10">Real-Time Wavefront</span>
                </div>
                
                <canvas id="interferenceCanvas" class="w-full h-[500px] rounded-[2.5rem] bg-black border-4 border-slate-900 shadow-2xl"></canvas>
                
                <!-- Screen Marker -->
                <div class="absolute right-4 top-1/2 -translate-y-1/2 flex flex-col items-center gap-1 opacity-50">
                    <div class="w-1 h-32 bg-indigo-500 rounded-full"></div>
                    <span class="[writing-mode:vertical-lr] text-[10px] font-bold tracking-[0.3em] uppercase text-indigo-400">Projection Screen</span>
                </div>
            </div>
        </div>
    </div>

    <script>
        const canvas = document.getElementById('interferenceCanvas');
        const ctx = canvas.getContext('2d');
        const dSlider = document.getElementById('dSlider');
        const lSlider = document.getElementById('lSlider');
        const dVal = document.getElementById('dVal');
        const lVal = document.getElementById('lVal');
        const resetBtn = document.getElementById('resetTime');

        let time = 0;
        const resolutionScale = 2; // Performance vs Quality

        function render() {
            const w = canvas.width = canvas.offsetWidth / resolutionScale;
            const h = canvas.height = canvas.offsetHeight / resolutionScale;
            
            const d = parseInt(dSlider.value);
            const wavelength = parseInt(lSlider.value);
            const k = (2 * Math.PI) / wavelength; // Wave number
            const omega = 0.12; // Angular frequency
            
            dVal.innerText = `${d} px`;
            lVal.innerText = `${wavelength} px`;

            // Position of the two slits (point sources)
            const r1 = { x: 20, y: h / 2 - d / 2 };
            const r2 = { x: 20, y: h / 2 + d / 2 };

            const imageData = ctx.createImageData(w, h);
            const pixels = imageData.data;

            const A = 60; // Amplitude constant

            for (let y = 0; y < h; y++) {
                for (let x = 0; x < w; x++) {
                    // Distances from both slits to current pixel
                    const dist1 = Math.sqrt((x - r1.x) ** 2 + (y - r1.y) ** 2) + 0.1;
                    const dist2 = Math.sqrt((x - r2.x) ** 2 + (y - r2.y) ** 2) + 0.1;

                    // u = (A/r1) * sin(kr1 - wt) + (A/r2) * sin(kr2 - wt)
                    const wave1 = (A / Math.sqrt(dist1)) * Math.sin(k * dist1 - time);
                    const wave2 = (A / Math.sqrt(dist2)) * Math.sin(k * dist2 - time);
                    
                    const totalU = wave1 + wave2;

                    // Color mapping
                    const index = (y * w + x) * 4;
                    const val = 128 + totalU * 1.5;
                    const clamped = Math.min(255, Math.max(0, val));

                    // Monochromatic indigo interference pattern
                    pixels[index] = clamped * 0.3;     // R
                    pixels[index + 1] = clamped * 0.4; // G
                    pixels[index + 2] = clamped;       // B
                    pixels[index + 3] = 255;           // A
                }
            }

            ctx.putImageData(imageData, 0, 0);

            // Draw Slit Indicators
            ctx.fillStyle = "white";
            ctx.beginPath();
            ctx.arc(r1.x, r1.y, 2, 0, Math.PI * 2);
            ctx.arc(r2.x, r2.y, 2, 0, Math.PI * 2);
            ctx.fill();

            time += omega;
            requestAnimationFrame(render);
        }

        resetBtn.onclick = () => time = 0;
        
        window.addEventListener('resize', () => {
            canvas.width = canvas.offsetWidth / resolutionScale;
            canvas.height = canvas.offsetHeight / resolutionScale;
        });

        render();
    </script>
</body>
</html>