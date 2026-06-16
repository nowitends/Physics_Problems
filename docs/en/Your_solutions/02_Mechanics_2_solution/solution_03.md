# Task 03 – Conservation of Energy in a Pendulum

## Problem Statement

A simple pendulum of length $L = 1.0 , \text{m}$ is released from an initial angle of $15^\circ$. Determine the speed of the pendulum bob at the lowest point of its motion.

## Theory

Mechanical energy is conserved in the pendulum motion (neglecting air resistance).

At the highest point:

* the pendulum has maximum potential energy and zero kinetic energy.

At the lowest point:

* the pendulum has zero potential energy (taking lowest point as reference) and maximum kinetic energy.

The energy conservation equation is:

$$
m g h = \frac{1}{2} m v^2
$$

The vertical height $h$ of the bob from the lowest point is given by geometry:

$$
h = L - L \cos\theta = L(1 - \cos\theta)
$$

## Step-by-Step Solution

### Step 1 – Compute the vertical height

Given:

* $L = 1.0 , \text{m}$
* $\theta = 15^\circ$

$$
h = 1.0 , (1 - \cos 15^\circ)
$$

Using

$$
\cos 15^\circ \approx 0.966
$$

$$
h = 1.0 \cdot (1 - 0.966)
$$

$$
h = 0.034 , \text{m}
$$

### Step 2 – Apply conservation of energy

$$
m g h = \frac{1}{2} m v^2
$$

Cancel $m$:

$$
g h = \frac{1}{2} v^2
$$

Solve for $v$:

$$
v = \sqrt{2 g h}
$$

### Step 3 – Substitute numerical values

$$
v = \sqrt{2 \cdot 9.8 \cdot 0.034}
$$

$$
v = \sqrt{0.6664}
$$

$$
v \approx 0.816 , \text{m/s}
$$

## Final Result

$$
v \approx 0.816 , \text{m/s}
$$

## Interpretation

The speed of the pendulum at the bottom depends only on the vertical height it has fallen.

Using the geometric formula $h = L(1 - \cos\theta)$ gives an exact height and ensures precise calculation, rather than relying on small-angle approximations.
