# Task 03 – Superposition Principle

## Problem Statement

Two waves are given by

$
y_1(x,t) = A \sin(kx - \omega t)
$

and

$
y_2(x,t) = A \sin(kx + \omega t)
$

Determine the equation of the resulting standing wave and identify the positions of the nodes.

---

## Theory

The principle of superposition states that when two waves overlap, the resultant displacement is the sum of the individual displacements:

$$
y(x,t) = y_1(x,t) + y_2(x,t)
$$

A trigonometric identity is used to combine the two sine functions:

$$
\sin \alpha + \sin \beta = 2 \sin\left(\frac{\alpha + \beta}{2}\right)\cos\left(\frac{\alpha - \beta}{2}\right)
$$

This identity allows transformation of two traveling waves into a standing wave form.

---

## Step-by-Step Solution

### Combine the Two Waves

The total displacement is

$$
y(x,t) = A \sin(kx - \omega t) + A \sin(kx + \omega t)
$$

Factor out $A$:

$$
y(x,t) = A \left[\sin(kx - \omega t) + \sin(kx + \omega t)\right]
$$

---

### Apply Trigonometric Identity

Let

$$
\alpha = kx - \omega t, \quad \beta = kx + \omega t
$$

Apply the identity:

$$
y(x,t) = 2A \sin\left(\frac{\alpha + \beta}{2}\right)\cos\left(\frac{\alpha - \beta}{2}\right)
$$

Substitute:

$$
\frac{\alpha + \beta}{2} = \frac{(kx - \omega t) + (kx + \omega t)}{2} = kx
$$

$$
\frac{\alpha - \beta}{2} = \frac{(kx - \omega t) - (kx + \omega t)}{2} = -\omega t
$$

Thus,

$$
y(x,t) = 2A \sin(kx)\cos(-\omega t)
$$

---

### Simplify Expression

Using the identity $\cos(-\theta) = \cos(\theta)$:

$$
y(x,t) = 2A \sin(kx)\cos(\omega t)
$$

---

### Determine Node Positions

Nodes occur where the displacement is always zero. This happens when

$$
\sin(kx) = 0
$$

The general solution is

$$
kx = n\pi
$$

Solve for position:

$$
x = \frac{n\pi}{k}
$$

Using the relation $k = \frac{2\pi}{\lambda}$:

$$
x = \frac{n\pi}{2\pi/\lambda}
$$

$$
x = \frac{n\lambda}{2}
$$

---

## Final Result

Standing wave equation:

$$
y(x,t) = 2A \sin(kx)\cos(\omega t)
$$

Node positions:

$$
x = \frac{n\lambda}{2}, \quad n = 0,1,2,3,\dots
$$

---

## Interpretation

The resulting wave is a standing wave formed by the interference of two waves traveling in opposite directions.

The term $\sin(kx)$ determines the spatial variation, while $\cos(\omega t)$ governs the time oscillation.

Nodes are fixed points where the displacement is always zero. These occur at regular intervals of $\frac{\lambda}{2}$ along the string.
