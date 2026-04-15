# Task 09 – Vector Lorentz Force

## Problem Statement

A proton moves with velocity

$$
\vec{v} = (2\hat{i} - 4\hat{j} + \hat{k}) , \text{m/s}
$$

in a magnetic field

$$
\vec{B} = (\hat{i} + 2\hat{j} - \hat{k}) , \text{T}
$$

Determine the magnitude of the magnetic force on the proton.

---

## Theory

### Magnetic Lorentz Force (Vector Form)

The magnetic force on a moving charge is

$$
\vec{F} = q (\vec{v} \times \vec{B})
$$

Magnitude:

$$
F = q |\vec{v} \times \vec{B}|
$$

For a proton:

$$
q = e = 1.6 \times 10^{-19} , \text{C}
$$

---

## Step-by-Step Solution

## Step 1: Compute Cross Product

Write vectors:

$$
\vec{v} =
\begin{pmatrix}
2 ,\ -4, \ 1
\end{pmatrix}
\quad , \quad
\vec{B} =
\begin{pmatrix}
1, \ 2, \ -1
\end{pmatrix}
$$

---

### Cross Product Formula

$$
\vec{v} \times \vec{B} =
\begin{pmatrix}
v_y B_z - v_z B_y, \
v_z B_x - v_x B_z, \
v_x B_y - v_y B_x
\end{pmatrix}
$$

---

### x-component

$$
(-4)(-1) - (1)(2) = 4 - 2 = 2
$$

---

### y-component

$$
(1)(1) - (2)(-1) = 1 + 2 = 3
$$

---

### z-component

$$
(2)(2) - (-4)(1) = 4 + 4 = 8
$$

---

Thus:

$$
\vec{v} \times \vec{B} = (2\hat{i} + 3\hat{j} + 8\hat{k})
$$

---

## Step 2: Magnitude of Cross Product

$$
|\vec{v} \times \vec{B}| = \sqrt{2^2 + 3^2 + 8^2}
$$

$$
= \sqrt{4 + 9 + 64}
$$

$$
= \sqrt{77}
$$

---

## Step 3: Magnetic Force

$$
F = q |\vec{v} \times \vec{B}|
$$

$$
F = (1.6 \times 10^{-19}) \sqrt{77}
$$

---

### Approximation

$$
\sqrt{77} \approx 8.77
$$

$$
F \approx (1.6 \times 10^{-19})(8.77)
$$

$$
F \approx 1.40 \times 10^{-18} , \text{N}
$$

---

## Final Result

$$
F \approx 1.4 \times 10^{-18} , \text{N}
$$

---

## Interpretation

* The force depends on the perpendicular component of velocity relative to the magnetic field
* The cross product determines how strongly the vectors are “misaligned”
* If vectors were parallel, force would be zero
* This force always acts perpendicular to both $\vec{v}$ and $\vec{B}$

This is the fundamental reason magnetic forces change direction but not speed.
