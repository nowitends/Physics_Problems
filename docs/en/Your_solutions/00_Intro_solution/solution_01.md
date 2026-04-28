# Section 0 — Mathematical Foundations
**Student:** Ali Kuyumcu

## 1. Vector Algebra
Given vectors in $\mathbb{R}^3$:
$\vec{a} = [2, 1, -3]$  
$\vec{b} = [4, -2, 1]$

### (a) Magnitude of each vector
* **Magnitude of $\vec{a}$:** $|\vec{a}| = \sqrt{2^2 + 1^2 + (-3)^2} = \sqrt{4+1+9} = \sqrt{14} \approx 3.74$
* **Magnitude of $\vec{b}$:** $|\vec{b}| = \sqrt{4^2 + (-2)^2 + 1^2} = \sqrt{16+4+1} = \sqrt{21} \approx 4.58$

### (b) Dot product $\vec{a} \cdot \vec{b}$
$\vec{a} \cdot \vec{b} = (2)(4) + (1)(-2) + (-3)(1) = 8 - 2 - 3 = 3$

### (c) Cross product $\vec{a} \times \vec{b}$

Using the formula $\vec{a} \times \vec{b} = [a_y b_z - a_z b_y, a_z b_x - a_x b_z, a_x b_y - a_y b_x]$:
* **x-component:** $(1)(1) - (-3)(-2) = 1 - 6 = -5$
* **y-component:** $(-3)(4) - (2)(1) = -12 - 2 = -14$
* **z-component:** $(2)(-2) - (1)(4) = -4 - 4 = -8$
**Result:** $\vec{a} \times \vec{b} = [-5, -14, -8]$

### (d) Angle between $\vec{a}$ and $\vec{b}$
$\theta = \arccos \left( \frac{\vec{a} \cdot \vec{b}}{|\vec{a}| |\vec{b}|} \right) = \arccos \left( \frac{3}{\sqrt{14}\sqrt{21}} \right) = \arccos \left( \frac{3}{\sqrt{294}} \right)$
**Result:** $\theta \approx 79.9^\circ$
