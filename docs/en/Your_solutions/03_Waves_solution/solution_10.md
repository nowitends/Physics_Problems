<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wave Source Superposition</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body { background-color: #020617; }
        #canvasContainer { cursor: crosshair; }
        .slider-thumb::-webkit-slider-thumb {
            -webkit-appearance: none;
            height: 16px;
            width: 16px;
            border-radius: 50%;
            background: #6366f1;
            cursor: pointer;
        }
    </style>
</head>
<body class="text-slate-300 font-sans p-4">

    <div class="max-w-5xl mx-auto space-y-4">
        <header class="flex flex-col md:flex-row md:items-center justify-between gap-4 bg-slate-900/50 p-6 rounded-3xl border border-slate-800">
            <div>
                <h1 class="text-2xl font-black text-white tracking-tight">Wave Interference Lab</h1>
                <p class="text-xs text-slate-500 font-mono">u(r,t) = Σ [ A / |r-r₀|ᵅ ] * sin(k|r-r₀| - ωt)</p>
            </div>
            
            <div class="flex flex-wrap gap-6 items-center">
                <div class="space-y-1">
                    <div class="flex justify-between text-[10px] font-bold text-slate-500 uppercase">Attenuation (α)</div>
                    <input type="range" id="alphaSlider" min="0" max="1" step="0.05" value="0.5" class="w-32 accent-indigo-500">
                    <div id="alphaVal" class="text-right text-xs text-indigo-400 font-mono">0.50</div>
                </div>
                <button id="clearBtn" class="px-4 py-2 bg-rose-600/20 hover:bg-rose-600/30 text-rose-400 text-xs font-bold rounded-xl border border-rose-600/40 transition-all">
                    CLEAR ALL
                </button>
            </div>
        </header>

        <div id="canvasContainer" class="relative group">
            <canvas id="waveCanvas" class="w-full rounded-3xl border-4 border-slate-900 shadow-2xl bg-black"></canvas>
            <div class="absolute bottom-4 left-6 pointer-events-none">
                <p class="text-white/50 text-[10px] font-bold uppercase tracking-widest">Click to Add Sources</p>
                <p id="sourceCount" class="text-indigo-400 text-xs font-mono">Sources: 1</p>
            </div>
        </div>

        <div class="bg-indigo-950/30 p-4 rounded-2xl border border-indigo-500/20 text-xs text-indigo-200/70 leading-relaxed">
            <b>Physics Note:</b> As α increases, the wave energy drops off faster with distance. When multiple sources are placed, they interfere constructively (bright) or destructively (dark), creating an interference pattern.
        </div>
    </div>

    <script>
        const canvas = document.getElementById('waveCanvas');
        const ctx = canvas.getContext('2d');
        const alphaSlider = document.getElementById('alphaSlider');
        const alphaVal = document.getElementById('alphaVal');
        const clearBtn = document.getElementById('clearBtn');
        const sourceCount = document.getElementById('sourceCount');

        let sources = [{x: 0, y: 0}]; // Initial source
        let time = 0;
        const scale = 2; // Resolution downscaling for performance
        
        // Physics constants
        const A = 120;     // Amplitude
        const k = 0.15;    // Wave number
        const omega = 0.1; // Angular frequency

        function resize() {
            canvas.width = canvas.offsetWidth / scale;
            canvas.height = (canvas.offsetWidth * 0.5) / scale;
            sources[0] = {x: canvas.width/2, y: canvas.height/2};
        }

        window.addEventListener('resize', resize);
        resize();

        canvas.addEventListener('mousedown', (e) => {
            const rect = canvas.getBoundingClientRect();
            const x = (e.clientX - rect.left) * (canvas.width / rect.width);
            const y = (e.clientY - rect.top) * (canvas.height / rect.height);
            sources.push({x, y});
            sourceCount.innerText = `Sources: ${sources.length}`;
        });

        clearBtn.onclick = () => {
            sources = [];
            sourceCount.innerText = `Sources: 0`;
        };

        function render() {
            const w = canvas.width;
            const h = canvas.height;
            const alpha = parseFloat(alphaSlider.value);
            alphaVal.innerText = alpha.toFixed(2);

            // Create ImageData for pixel-level manipulation
            const imageData = ctx.createImageData(w, h);
            const data = imageData.data;

            for (let y = 0; y < h; y++) {
                for (let x = 0; x < w; x++) {
                    let u = 0;

                    // Superposition logic: Sum waves from all sources
                    for (let s of sources) {
                        const dx = x - s.x;
                        const dy = y - s.y;
                        const r = Math.sqrt(dx * dx + dy * dy) + 0.1; // +0.1 to avoid div by zero
                        
                        // u(r,t) = (A / r^α) * sin(k*r - ω*t)
                        u += (A / Math.pow(r, alpha)) * Math.sin(k * r - time);
                    }

                    const idx = (y * w + x) * 4;
                    
                    // Map displacement u to color
                    // We use a blue-to-white-to-indigo palette
                    const val = Math.min(255, Math.max(0, 128 + u));
                    data[idx] = val * 0.4;     // R
                    data[idx + 1] = val * 0.6; // G
                    data[idx + 2] = val;       // B
                    data[idx + 3] = 255;       // A
                }
            }

            ctx.putImageData(imageData, 0, 0);

            // Draw Source Dots
            ctx.fillStyle = "white";
            for(let s of sources) {
                ctx.beginPath();
                ctx.arc(s.x, s.y, 1.5, 0, Math.PI*2);
                ctx.fill();
            }

            time += omega;
            requestAnimationFrame(render);
        }

        render();
    </script>
</body>
</html>