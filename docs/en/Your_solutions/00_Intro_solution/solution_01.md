# Task 01 – Vector Algebra in 3D

## Problem Statement

Given two vectors in 3D space:

$$
\vec{a} = [2, 1, -3], \quad \vec{b} = [4, -2, 1]
$$

Calculate:

a) The magnitude of each vector.

b) The dot product $\vec{a} \cdot \vec{b}$.

c) The cross product $\vec{a} \times \vec{b}$.

d) The angle between the vectors $\vec{a}$ and $\vec{b}$.

---

## Theory

**Vectors in 3D space** have both magnitude and direction, represented by three components along the $x$, $y$, and $z$ axes.

Key concepts:

1. **Magnitude of a vector** $\vec{v} = [v_x, v_y, v_z]$:

$$
|\vec{v}| = \sqrt{v_x^2 + v_y^2 + v_z^2}
$$

2. **Dot product** of two vectors $\vec{a}$ and $\vec{b}$:

$$
\vec{a} \cdot \vec{b} = a_x b_x + a_y b_y + a_z b_z
$$

The dot product is also related to the angle $\theta$ between the vectors:

$$
\vec{a} \cdot \vec{b} = |\vec{a}| |\vec{b}| \cos \theta
$$

3. **Cross product** of two vectors $\vec{a}$ and $\vec{b}$:

The cross product produces a vector perpendicular to both $\vec{a}$ and $\vec{b}$, with magnitude

$$
|\vec{a} \times \vec{b}| = |\vec{a}| |\vec{b}| \sin \theta
$$

and direction given by the right-hand rule.

The formula for the cross product in 3D is:

$$
\vec{a} \times \vec{b} =
\begin{pmatrix}
a_y b_z - a_z b_y \
a_z b_x - a_x b_z \
a_x b_y - a_y b_x
\end{pmatrix}
$$

4. **Angle between vectors**:

$$
\theta = \arccos \left( \frac{\vec{a} \cdot \vec{b}}{|\vec{a}| |\vec{b}|} \right)
$$

---

## Step-by-Step Solution

### Step 1 — Magnitude of Each Vector

For $\vec{a} = [2, 1, -3]$:

$$
|\vec{a}| = \sqrt{2^2 + 1^2 + (-3)^2}
$$

$$
|\vec{a}| = \sqrt{4 + 1 + 9}
$$

$$
|\vec{a}| = \sqrt{14} \approx 3.742
$$

For $\vec{b} = [4, -2, 1]$:

$$
|\vec{b}| = \sqrt{4^2 + (-2)^2 + 1^2}
$$

$$
|\vec{b}| = \sqrt{16 + 4 + 1}
$$

$$
|\vec{b}| = \sqrt{21} \approx 4.583
$$

---

### Step 2 — Dot Product

$$
\vec{a} \cdot \vec{b} = (2)(4) + (1)(-2) + (-3)(1)
$$

$$
\vec{a} \cdot \vec{b} = 8 - 2 - 3
$$

$$
\vec{a} \cdot \vec{b} = 3
$$

---

### Step 3 — Cross Product (Detailed)

The cross product formula is:

$$
\vec{a} \times \vec{b} =
\begin{pmatrix}
a_y b_z - a_z b_y \
a_z b_x - a_x b_z \
a_x b_y - a_y b_x
\end{pmatrix}
$$

Substitute the components of $\vec{a} = [2, 1, -3]$ and $\vec{b} = [4, -2, 1]$:

1. **x-component**:

$$
(\vec{a} \times \vec{b})_x = a_y b_z - a_z b_y
$$

$$
= (1)(1) - (-3)(-2)
$$

$$
= 1 - 6
$$

$$
= -5
$$

2. **y-component**:

$$
(\vec{a} \times \vec{b})_y = a_z b_x - a_x b_z
$$

$$
= (-3)(4) - (2)(1)
$$

$$
= -12 - 2
$$

$$
= -14
$$

3. **z-component**:

$$
(\vec{a} \times \vec{b})_z = a_x b_y - a_y b_x
$$

$$
= (2)(-2) - (1)(4)
$$

$$
= -4 - 4
$$

$$
= -8
$$

Thus, the cross product vector is:

$$
\vec{a} \times \vec{b} = [-5, -14, -8]
$$

**Magnitude of cross product**:

$$
|\vec{a} \times \vec{b}| = \sqrt{(-5)^2 + (-14)^2 + (-8)^2}
$$

$$
|\vec{a} \times \vec{b}| = \sqrt{25 + 196 + 64}
$$

$$
|\vec{a} \times \vec{b}| = \sqrt{285} \approx 16.881
$$

---

### Step 4 — Angle Between Vectors

The angle $\theta$ is given by

$$
\theta = \arccos \left( \frac{\vec{a} \cdot \vec{b}}{|\vec{a}| |\vec{b}|} \right)
$$

Substitute values:

$$
\theta = \arccos \left( \frac{3}{\sqrt{14} \cdot \sqrt{21}} \right)
$$

$$
\theta = \arccos \left( \frac{3}{\sqrt{294}} \right)
$$

$$
\theta = \arccos \left( \frac{3}{17.146} \right)
$$

$$
\theta \approx \arccos(0.175)
$$

$$
\theta \approx 80.0^\circ
$$

---

## Final Result

* Magnitudes:

$$
|\vec{a}| = \sqrt{14} \approx 3.742, \quad |\vec{b}| = \sqrt{21} \approx 4.583
$$

* Dot product:

$$
\vec{a} \cdot \vec{b} = 3
$$

* Cross product:

$$
\vec{a} \times \vec{b} = [-5, -14, -8], \quad |\vec{a} \times \vec{b}| \approx 16.881
$$

* Angle between vectors:

$$
\theta \approx 80.0^\circ
$$

---

## Interpretation

* The **magnitudes** represent the lengths of the vectors in 3D space.
* The **dot product** indicates a small positive correlation; vectors are almost perpendicular.
* The **cross product** gives a vector perpendicular to both $\vec{a}$ and $\vec{b}$, with magnitude showing the area of the parallelogram formed by the two vectors.
* The **angle** of approximately $80^\circ$ confirms that the vectors are nearly orthogonal but not exactly at right angles.

The detailed cross product steps clarify how each component is calculated and why the resulting vector points perpendicular to the plane containing $\vec{a}$ and $\vec{b}$.
