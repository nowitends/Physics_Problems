No problem! Let’s break these down step-by-step so the logic behind the math is crystal clear.

---

## 1. Vector Algebra

**Given:** $\vec{a} = [2, 1, -3]$ and $\vec{b} = [4, -2, 1]$

* **a) Magnitude:** Think of this as the "length" of the arrow using the 3D Pythagorean theorem: $\sqrt{x^2 + y^2 + z^2}$.
* $|\vec{a}| = \sqrt{2^2 + 1^2 + (-3)^2} = \sqrt{4 + 1 + 9} = \mathbf{\sqrt{14}}$
* $|\vec{b}| = \sqrt{4^2 + (-2)^2 + 1^2} = \sqrt{16 + 4 + 1} = \mathbf{\sqrt{21}}$


* **b) Dot Product ($\vec{a} \cdot \vec{b}$):** Multiply the corresponding parts and add them up. It tells you how much one vector goes in the direction of the other.
* $(2 \times 4) + (1 \times -2) + (-3 \times 1) = 8 - 2 - 3 = \mathbf{3}$


* **c) Cross Product ($\vec{a} \times \vec{b}$):** This results in a new vector perpendicular to both $\vec{a}$ and $\vec{b}$. We use the determinant method:
* $x = (1 \times 1) - (-3 \times -2) = 1 - 6 = -5$
* $y = -[(2 \times 1) - (-3 \times 4)] = -(2 + 12) = -14$
* $z = (2 \times -2) - (1 \times 4) = -4 - 4 = -8$
* **Result:** $\mathbf{[-5, -14, -8]}$


* **d) Angle ($\theta$):** Use the definition $\vec{a} \cdot \vec{b} = |\vec{a}||\vec{b}| \cos(\theta)$.
* $3 = \sqrt{14} \cdot \sqrt{21} \cdot \cos(\theta)$
* $\cos(\theta) = \frac{3}{\sqrt{294}} \approx 0.175$
* $\theta = \arccos(0.175) \approx \mathbf{79.9^\circ}$



---

## 2. Systems of Equations

**Equations:** (1) $2x + 3y = 12$ and (2) $x - y = 1$

1. **Isolate $x$ in Eq 2:** $x = y + 1$.
2. **Substitute into Eq 1:** $2(y + 1) + 3y = 12$.
3. **Simplify:** $2y + 2 + 3y = 12 \implies 5y + 2 = 12 \implies 5y = 10$.
4. **Solve:** $y = 2$.
5. **Plug back for $x$:** $x = 2 + 1 = 3$.
**Solution:** **(3, 2)**

---

## 3. Proportionality

**Formula:** $F = G \frac{m_1 m_2}{r^2}$

* If $r$ doubles ($2r$), the denominator becomes $(2r)^2 = 4r^2$ (Force becomes $1/4$).
* If $m_1$ is halved ($0.5m_1$) and $m_2$ is halved ($0.5m_2$), the numerator becomes $0.5 \times 0.5 = 0.25$ (Force becomes $1/4$).
* **Combine them:** $\frac{1}{4} (\text{from masses}) \times \frac{1}{4} (\text{from distance}) = \mathbf{1/16}$.
The new force is **1/16** of the original.

---

## 4. Rearranging Formulas

**Goal:** Isolate $g$ in $T = 2\pi \sqrt{\frac{L}{g}}$

1. **Divide by $2\pi$:** $\frac{T}{2\pi} = \sqrt{\frac{L}{g}}$
2. **Square both sides:** $\frac{T^2}{4\pi^2} = \frac{L}{g}$
3. **Flip both sides (reciprocal):** $\frac{4\pi^2}{T^2} = \frac{g}{L}$
4. **Multiply by $L$:** $\mathbf{g = \frac{4\pi^2 L}{T^2}}$

---

## 5. Trigonometry

**Vector $\vec{A}$:** Magnitude $15$, angle $60^\circ$.

* **Horizontal ($A_x$):** $\text{Adjacent} = \text{Hypotenuse} \times \cos(\theta)$
* $15 \cos(60^\circ) = 15 \times 0.5 = \mathbf{7.5}$


* **Vertical ($A_y$):** $\text{Opposite} = \text{Hypotenuse} \times \sin(\theta)$
* $15 \sin(60^\circ) = 15 \times \frac{\sqrt{3}}{2} \approx \mathbf{12.99}$



---

## 6. Function Analysis

**Function:** $f(x) = 3x^2 - 12x + 7$

1. **Find the derivative ($f'$):** $f'(x) = 6x - 12$.
2. **Find critical points:** Set $f'(x) = 0 \implies 6x = 12 \implies \mathbf{x = 2}$.
3. **Check if Max or Min:** The second derivative $f''(x) = 6$. Since it's positive, the graph curves upward like a smile. This is a **local minimum**.
4. **Find the y-value:** $f(2) = 3(2)^2 - 12(2) + 7 = 12 - 24 + 7 = \mathbf{-5}$.

---

## 7. Logic & Series

**The Trick:** Don't calculate every single flight of the fly. Just look at the **total time**.

1. **Time:** The bicycle travels 10 meters at 1 m/s. It will hit the wall in **10 seconds**.
2. **The Fly:** The fly is flying at a constant 2 m/s for that entire 10 seconds (it doesn't matter how many times it turns).
3. **Distance:** $\text{Speed} \times \text{Time} = 2\text{ m/s} \times 10\text{ s} = \mathbf{20 \text{ meters}}$.

---

## 8. Definite Integrals

**Problem:** $\int_{0}^{\pi} \sin(x) dx$

1. **Anti-derivative:** The integral of $\sin(x)$ is $-\cos(x)$.
2. **Evaluate at boundaries:** $[-\cos(\pi)] - [-\cos(0)]$.
3. **Calculate:** $-(-1) - (-1) = 1 + 1 = \mathbf{2}$.

---

## 9. Optimization Problem

**Curve:** $y = 3 - x^2$. **Area of rectangle:** $A = x \cdot y$.

1. **Substitute $y$:** $A(x) = x(3 - x^2) = 3x - x^3$.
2. **Differentiate:** $A'(x) = 3 - 3x^2$.
3. **Set to zero:** $3 - 3x^2 = 0 \implies x^2 = 1 \implies \mathbf{x = 1}$.
4. **Find dimensions:** If $x = 1$, then $y = 3 - (1)^2 = \mathbf{2}$.
The dimensions for maximum area are **1 unit wide by 2 units high**.

---

## 10. Infinite Series

The ant's path is a alternating series for $x$ and $y$.

* **x-axis:** $1 - 1/3 + 1/5 - 1/7 \dots$ This is the famous **Leibniz formula for $\pi/4$**.
* **y-axis:** $1/2 - 1/4 + 1/6 - 1/8 \dots$ Factor out $1/2$: $\frac{1}{2}(1 - 1/2 + 1/3 - 1/4 \dots)$. The part in the parentheses is the natural log of 2 ($\ln 2$). So, $y = \mathbf{\frac{\ln 2}{2}}$.
**Final Position:** $(\frac{\pi}{4}, \frac{\ln 2}{2}) \approx \mathbf{(0.785, 0.347)}$

---

Would you like me to generate a practice quiz based on these topics to see how well you've got them down?