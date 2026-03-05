## Problem 1. Vector Algebra (step by step)

Given  
$\vec{a}=[2,1,-3]$ and $\vec{b}=[4,-2,1]$.

---

# Vector Operations in 3D

Given two vectors in 3D space:

$$
\vec{a} = [2, 1, -3]
$$

$$
\vec{b} = [4, -2, 1]
$$

---

# a) Magnitude of Each Vector

The magnitude (length) of a vector is given by:

$$
|\vec{v}| = \sqrt{x^2 + y^2 + z^2}
$$

### Magnitude of **a**

$$
|\vec{a}| = \sqrt{2^2 + 1^2 + (-3)^2}
$$

$$
|\vec{a}| = \sqrt{4 + 1 + 9}
$$

$$
|\vec{a}| = \sqrt{14}
$$

### Magnitude of **b**

$$
|\vec{b}| = \sqrt{4^2 + (-2)^2 + 1^2}
$$

$$
|\vec{b}| = \sqrt{16 + 4 + 1}
$$

$$
|\vec{b}| = \sqrt{21}
$$

**Results**

$$
|\vec{a}| = \sqrt{14}, \qquad |\vec{b}| = \sqrt{21}
$$

---

# b) Dot Product

The dot product of two vectors is defined as:

$$
\vec{a} \cdot \vec{b} =
a_x b_x + a_y b_y + a_z b_z
$$

Substitute the vector components:

$$
\vec{a} \cdot \vec{b}
=
(2)(4) + (1)(-2) + (-3)(1)
$$

$$
= 8 - 2 - 3
$$

$$
= 3
$$

**Result**

$$
\vec{a} \cdot \vec{b} = 3
$$

---

# c) Cross Product

The cross product is computed using the determinant:

$$
\vec{a} \times \vec{b} =
\begin{vmatrix}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
2 & 1 & -3 \\
4 & -2 & 1
\end{vmatrix}
$$

Expanding the determinant:

$$
=
\mathbf{i}(1 \cdot 1 - (-3)(-2))
-
\mathbf{j}(2 \cdot 1 - (-3)(4))
+
\mathbf{k}(2(-2) - 1(4))
$$

Now compute each term:

$$
= \mathbf{i}(1 - 6) - \mathbf{j}(2 + 12) + \mathbf{k}(-4 - 4)
$$

$$
= -5\mathbf{i} - 14\mathbf{j} - 8\mathbf{k}
$$

**Result**

$$
\vec{a} \times \vec{b} = [-5, -14, -8]
$$

---

# d) Angle Between the Vectors

The angle between vectors is given by:

$$
\cos\theta =
\frac{\vec{a} \cdot \vec{b}}
{|\vec{a}| |\vec{b}|}
$$

Substitute the known values:

$$
\cos\theta =
\frac{3}{\sqrt{14}\sqrt{21}}
$$

Combine the square roots:

$$
\cos\theta =
\frac{3}{\sqrt{294}}
$$

Since

$$
\sqrt{294} = 7\sqrt{6}
$$

we get

$$
\cos\theta =
\frac{3}{7\sqrt{6}}
$$

Rationalizing the denominator:

$$
\cos\theta =
\frac{\sqrt{6}}{14}
$$

Therefore:

$$
\theta = \arccos\left(\frac{\sqrt{6}}{14}\right)
$$

Approximate value:

$$
\theta \approx 80^\circ
$$

---

# Final Results

**Magnitudes**

$$
|\vec{a}| = \sqrt{14}, \qquad |\vec{b}| = \sqrt{21}
$$

**Dot Product**

$$
\vec{a} \cdot \vec{b} = 3
$$

**Cross Product**

$$
\vec{a} \times \vec{b} = [-5, -14, -8]
$$

**Angle Between Vectors**

$$
\theta = \arccos\left(\frac{\sqrt{6}}{14}\right) \approx 80^\circ
$$