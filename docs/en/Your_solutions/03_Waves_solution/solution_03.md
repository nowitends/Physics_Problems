## 3. Superposition Principle – Formal Step-by-Step Solution

### **Problem Statement**
Consider two harmonic waves traveling in opposite directions along the same medium, described by the following wave functions:
$$y_1(x,t) = A \sin(kx - \omega t)$$
$$y_2(x,t) = A \sin(kx + \omega t)$$

1. Derive the equation of the resulting **standing wave**.
2. Identify the mathematical positions of the **nodes** (points of zero displacement).

---

### **Step 1: Application of the Superposition Principle**
The Principle of Superposition states that when two or more waves overlap in the same medium, the net displacement at any point is the algebraic sum of the individual displacements:
$$y_{net}(x,t) = y_1(x,t) + y_2(x,t)$$

Substituting the given functions:
$$y_{net}(x,t) = A \sin(kx - \omega t) + A \sin(kx + \omega t)$$

---

### **Step 2: Trigonometric Derivation**
To simplify the sum of two sine functions, we use the standard trigonometric sum-to-product identity:
$$\sin(\alpha) + \sin(\beta) = 2 \sin\left(\frac{\alpha + \beta}{2}\right) \cos\left(\frac{\alpha - \beta}{2}\right)$$

Let $\alpha = kx + \omega t$ and $\beta = kx - \omega t$:
1.  **Sum ($\alpha + \beta$):** $(kx + \omega t) + (kx - \omega t) = 2kx$
2.  **Difference ($\alpha - \beta$):** $(kx + \omega t) - (kx - \omega t) = 2\omega t$

Plugging these into the identity:
$$y_{net}(x,t) = 2A \sin\left(\frac{2kx}{2}\right) \cos\left(\frac{2\omega t}{2}\right)$$
$$y_{net}(x,t) = \mathbf{2A \sin(kx) \cos(\omega t)}$$

---

### **Step 3: Identification of Node Positions**
**Nodes** are specific points in space ($x$) where the displacement is always zero, regardless of the time ($t$). This occurs when the spatial part of the standing wave equation is zero:
$$2A \sin(kx) = 0 \implies \sin(kx) = 0$$

The sine function is zero at integer multiples of $\pi$:
$$kx = n\pi \quad \text{where } n = 0, 1, 2, 3, \dots$$

---

### **Step 4: Expressing Nodes in Terms of Wavelength ($\lambda$)**
Since the wave number is defined as $k = \frac{2\pi}{\lambda}$, we substitute this into the node condition:
$$\left( \frac{2\pi}{\lambda} \right) x = n\pi$$

Solving for $x$:
1. Cancel $\pi$ from both sides: $\frac{2x}{\lambda} = n$
2. Isolate $x$:
$$x = n \frac{\lambda}{2} \quad (n = 0, 1, 2, \dots)$$

---

### **Step 5: Final Results Summary**
| Feature | Mathematical Expression |
| :--- | :--- |
| **Resultant Wave Equation** | $y(x,t) = 2A \sin(kx) \cos(\omega t)$ |
| **Node Positions** | $x = 0, \frac{\lambda}{2}, \lambda, \frac{3\lambda}{2}, \dots$ |
| **Antinode Positions** | $x = \frac{\lambda}{4}, \frac{3\lambda}{4}, \frac{5\lambda}{4}, \dots$ |

---

### **Step 6: Physical Analysis**
* **Stationary Pattern:** Unlike traveling waves, the $x$ and $t$ variables are separated ($kx$ is inside sine, $\omega t$ is inside cosine). This means the wave pattern oscillates in place but does not move left or right.
* **Amplitude:** The term $2A \sin(kx)$ acts as a position-dependent amplitude. At nodes, this amplitude is $0$; at antinodes, it is a maximum of $2A$.
