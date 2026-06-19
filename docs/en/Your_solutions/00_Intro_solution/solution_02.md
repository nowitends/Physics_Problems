Here are the full solutions for **Section 0: Mathematical Foundations** formatted with clear 

$$\LaTeX$$

 and Markdown for easy reading.

---

## **1. Vector Algebra**

Given $\vec{a} = [2, 1, -3]$ and $\vec{b} = [1, -2, 1]$:

### **a) Magnitude of each vector**

$$|\vec{a}| = \sqrt{2^2 + 1^2 + (-3)^2} = \sqrt{4 + 1 + 9} = \mathbf{\sqrt{14}}$$

$$|\vec{b}| = \sqrt{1^2 + (-2)^2 + 1^2} = \sqrt{1 + 4 + 1} = \mathbf{\sqrt{6}}$$

### **b) Dot Product ($\vec{a} \cdot \vec{b}$)**

$$\vec{a} \cdot \vec{b} = (2)(1) + (1)(-2) + (-3)(1) = 2 - 2 - 3 = \mathbf{-3}$$

### **c) Cross Product ($\vec{a} \times \vec{b}$)**

Using the determinant formula:


$$\vec{a} \times \vec{b} = \begin{bmatrix} (1)(1) - (-3)(-2) \\ (-3)(1) - (2)(1) \\ (2)(-2) - (1)(1) \end{bmatrix} = \begin{bmatrix} 1 - 6 \\ -3 - 2 \\ -4 - 1 \end{bmatrix} = \mathbf{[-5, -5, -5]}$$

### **d) Angle ($\theta$) between $\vec{a}$ and $\vec{b}$**

$$\cos \theta = \frac{\vec{a} \cdot \vec{b}}{|\vec{a}||\vec{b}|} = \frac{-3}{\sqrt{14}\sqrt{6}} = \frac{-3}{\sqrt{84}}$$

$$\theta = \arccos\left(\frac{-3}{\sqrt{84}}\right) \approx \mathbf{109.1^\circ}$$

---

## **2. Systems of Equations**

Solve: $2x + 3y = 12$ and $x - y = 1$:

1. From the second equation: $x = y + 1$.
2. Substitute into the first: 
$$2(y + 1) + 3y = 12 \implies 5y + 2 = 12 \implies 5y = 10 \implies \mathbf{y = 2}$$


3. Solving for $x$: $x = 2 + 1 \implies \mathbf{x = 3}$.

---

## **3. Proportionality**

Using $F = G\frac{m_1 m_2}{r^2}$. If $r' = 2r$, $m_1' = \frac{1}{2}m_1$, and $m_2' = \frac{1}{2}m_2$:


$$F' = G\frac{(\frac{1}{2}m_1)(\frac{1}{2}m_2)}{(2r)^2} = G\frac{\frac{1}{4}m_1 m_2}{4r^2} = \frac{1}{16} \left( G\frac{m_1 m_2}{r^2} \right) = \mathbf{\frac{1}{16}F}$$

---

## **4. Rearranging Formulas**

Solve $T = 2\pi\sqrt{\frac{L}{g}}$ for $g$:


$$\frac{T}{2\pi} = \sqrt{\frac{L}{g}} \implies \frac{T^2}{4\pi^2} = \frac{L}{g} \implies \mathbf{g = \frac{4\pi^2 L}{T^2}}$$

---

## **6. Function Analysis**

For $f(x) = 3x^2 - 12x + 7$:

1. Find the derivative: $f'(x) = 6x - 12$.
2. Set to zero: $6x - 12 = 0 \implies \mathbf{x = 2}$.
3. Second derivative check: $f''(x) = 6$. Since $6 > 0$, it is a **local minimum**.
4. $f(2) = 3(2)^2 - 12(2) + 7 = \mathbf{-5}$.

---

## **8. Definite Integrals**

Area under $f(x) = \sin(x)$ from $x=0$ to $x=\pi$:


$$\int_{0}^{\pi} \sin(x) dx = \left[ -\cos(x) \right]_{0}^{\pi} = -\cos(\pi) - (-\cos(0)) = -(-1) - (-1) = \mathbf{2}$$

---

## **9. Optimization Problem**

Area $A = x \cdot y$ where $y = 3 - x^2$:


$$A(x) = x(3 - x^2) = 3x - x^3$$

$$A'(x) = 3 - 3x^2 = 0 \implies x^2 = 1 \implies \mathbf{x = 1}$$


If $x = 1$, then $y = 3 - (1)^2 = \mathbf{2}$. Dimensions for max area: **$x=1, y=2$**.

---

## **10. Infinite Series**

An ant moves $1$ m E, $1/2$ m N, $1/3$ m W, $1/4$ m S...

* **East/West ($x$):** $1 - \frac{1}{3} + \frac{1}{5} - \dots = \arctan(1) = \mathbf{\frac{\pi}{4}}$
* **North/South ($y$):** $\frac{1}{2} - \frac{1}{4} + \frac{1}{6} - \dots = \frac{1}{2}(1 - \frac{1}{2} + \frac{1}{3} - \dots) = \frac{1}{2}\ln(2)$
**Final Position:** 
$$\mathbf{\left(\frac{\pi}{4}, \frac{\ln 2}{2}\right)}$$



Would you like me to put these into a single Python cell for your Colab notebook?