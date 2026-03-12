# Section 0 — Mathematical Foundations  
## 1. Vector Algebra

We are given two vectors in $\mathbb{R}^3$:

$$
\vec{a} = [2,\,1,\,-3], \qquad \vec{b} = [4,\,-2,\,1]
$$

---

## Necessary definitions and formulas

### 1) Magnitude (length) of a vector
For $\vec{v} = [v_x, v_y, v_z]$,

$$
|\vec{v}| = \sqrt{v_x^2 + v_y^2 + v_z^2}
$$

### 2) Dot product
For $\vec{a} = [a_x,a_y,a_z]$ and $\vec{b} = [b_x,b_y,b_z]$,

$$
\vec{a}\cdot\vec{b} = a_x b_x + a_y b_y + a_z b_z
$$

### 3) Cross product
For $\vec{a} = [a_x,a_y,a_z]$ and $\vec{b} = [b_x,b_y,b_z]$,

$$
\vec{a}\times\vec{b} =
\begin{bmatrix}
a_y b_z - a_z b_y \\
a_z b_x - a_x b_z \\
a_x b_y - a_y b_x
\end{bmatrix}
$$

### 4) Angle between two vectors
If $\theta$ is the angle between $\vec{a}$ and $\vec{b}$, then

$$
\vec{a}\cdot\vec{b} = |\vec{a}|\,|\vec{b}| \cos\theta
$$

So,

$$
\theta = \arccos\!\left(\frac{\vec{a}\cdot\vec{b}}{|\vec{a}|\,|\vec{b}|}\right)
$$

---

## (a) Magnitude of each vector

### Magnitude of $\vec{a}$
Using $|\vec{a}| = \sqrt{2^2 + 1^2 + (-3)^2}$:

$$
|\vec{a}| = \sqrt{4 + 1 + 9} = \sqrt{14}
$$

### Magnitude of $\vec{b}$
Using $|\vec{b}| = \sqrt{4^2 + (-2)^2 + 1^2}$:

$$
|\vec{b}| = \sqrt{16 + 4 + 1} = \sqrt{21}
$$

**Answer (a):**

$$
|\vec{a}|=\sqrt{14}, \qquad |\vec{b}|=\sqrt{21}
$$

---

## (b) Dot product $\vec{a}\cdot\vec{b}$

Compute component-by-component:

$$
\vec{a}\cdot\vec{b} = (2)(4) + (1)(-2) + (-3)(1)
$$

$$
\vec{a}\cdot\vec{b} = 8 - 2 - 3 = 3
$$

**Answer (b):**

$$
\vec{a}\cdot\vec{b} = 3
$$

---

## (c) Cross product $\vec{a}\times\vec{b}$

Let $\vec{a}=[2,1,-3]$ and $\vec{b}=[4,-2,1]$.

### $x$-component
$$
(\vec{a}\times\vec{b})_x = a_y b_z - a_z b_y = (1)(1) - (-3)(-2) = 1 - 6 = -5
$$

### $y$-component
$$
(\vec{a}\times\vec{b})_y = a_z b_x - a_x b_z = (-3)(4) - (2)(1) = -12 - 2 = -14
$$

### $z$-component
$$
(\vec{a}\times\vec{b})_z = a_x b_y - a_y b_x = (2)(-2) - (1)(4) = -4 - 4 = -8
$$

So,

$$
\vec{a}\times\vec{b} = [-5,\,-14,\,-8]
$$

**Answer (c):**

$$
\vec{a}\times\vec{b} = [-5,\,-14,\,-8]
$$

---

## (d) Angle between $\vec{a}$ and $\vec{b}$

Use

$$
\theta = \arccos\!\left(\frac{\vec{a}\cdot\vec{b}}{|\vec{a}|\,|\vec{b}|}\right)
$$

We already found:
- $\vec{a}\cdot\vec{b} = 3$
- $|\vec{a}| = \sqrt{14}$
- $|\vec{b}| = \sqrt{21}$

Substitute:

$$
\theta = \arccos\!\left(\frac{3}{\sqrt{14}\sqrt{21}}\right)
$$

Combine the radicals:

$$
\sqrt{14}\sqrt{21}=\sqrt{294}
$$

So the exact form is:

$$
\theta = \arccos\!\left(\frac{3}{\sqrt{294}}\right)
$$

Optional numeric approximation:
- $\sqrt{294}\approx 17.146$
- $\frac{3}{\sqrt{294}}\approx 0.175$

So,

$$
\theta \approx \arccos(0.175)\approx 1.395\text{ rad}\approx 79.9^\circ
$$

**Answer (d):**

$$
\theta = \arccos\!\left(\frac{3}{\sqrt{294}}\right)\approx 79.9^\circ
$$

---

## Final answers (summary)

$$
|\vec{a}|=\sqrt{14}, \qquad |\vec{b}|=\sqrt{21}
$$

$$
\vec{a}\cdot\vec{b}=3
$$

$$
\vec{a}\times\vec{b}=[-5,\,-14,\,-8]
$$

$$
\theta=\arccos\!\left(\frac{3}{\sqrt{294}}\right)\approx 79.9^\circ
$$

My solution checked
