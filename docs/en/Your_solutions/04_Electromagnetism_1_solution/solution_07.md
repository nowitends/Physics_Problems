# Task 07 – Cyclotron Motion of an Electron

## Problem Statement

An electron is accelerated from rest through a potential difference of $5000 , \text{V}$. It then enters a uniform magnetic field of magnitude $B = 0.1 , \text{T}$, perpendicular to its velocity.

Determine the radius of the circular path followed by the electron.

---

## Theory

### Energy Gain from Electric Potential

When a charge $q$ is accelerated through a potential difference $V$, the gained kinetic energy is

$$
\frac{1}{2}mv^2 = qV
$$

---

### Motion in a Magnetic Field

When a charged particle enters a magnetic field perpendicular to its velocity, it experiences a magnetic force

$$
F = qvB
$$

This force acts as centripetal force:

$$
qvB = \frac{mv^2}{r}
$$

---

### Radius of Circular Motion

From the above relation:

$$
r = \frac{mv}{qB}
$$

---

## Step-by-Step Solution

## Step 1: Velocity from Acceleration

Energy conservation:

$$
\frac{1}{2}mv^2 = eV
$$

Solve for $v$:

$$
v = \sqrt{\frac{2eV}{m}}
$$

Substitute values:

* $e = 1.6 \times 10^{-19}$
* $V = 5000$
* $m = 9.11 \times 10^{-31}$

---

### Compute inside root

$$
2eV = 2 \cdot (1.6 \times 10^{-19}) \cdot 5000
$$

$$
= 1.6 \times 10^{-15}
$$

---

### Velocity

$$
v = \sqrt{\frac{1.6 \times 10^{-15}}{9.11 \times 10^{-31}}}
$$

$$
v = \sqrt{1.76 \times 10^{15}}
$$

$$
v \approx 4.2 \times 10^{7} , \text{m/s}
$$

---

## Step 2: Radius of Circular Path

$$
r = \frac{mv}{eB}
$$

Substitute:

$$
r = \frac{(9.11 \times 10^{-31})(4.2 \times 10^7)}{(1.6 \times 10^{-19})(0.1)}
$$

---

### Numerator

$$
9.11 \times 10^{-31} \cdot 4.2 \times 10^7 = 3.83 \times 10^{-23}
$$

---

### Denominator

$$
1.6 \times 10^{-19} \cdot 0.1 = 1.6 \times 10^{-20}
$$

---

### Final Radius

$$
r = \frac{3.83 \times 10^{-23}}{1.6 \times 10^{-20}}
$$

$$
r \approx 2.39 \times 10^{-3} , \text{m}
$$

---

## Final Result

$$
r \approx 2.4 \times 10^{-3} , \text{m}
$$

---

## Interpretation

* The electron gains kinetic energy from the electric field
* The magnetic field forces circular motion
* Higher velocity increases radius
* Stronger magnetic field decreases radius

The resulting path is a tight circle due to the electron’s small mass and strong magnetic interaction.
