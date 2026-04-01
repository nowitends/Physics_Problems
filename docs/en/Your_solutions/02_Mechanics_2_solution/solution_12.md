# Task 12 – Work and Energy with a Constant Force

## Problem Statement

A body of mass $m = 2\ \mathrm{kg}$ is subjected to a constant force

$$
\vec F = [6, 2]\ \mathrm{N}
$$

with initial conditions

$$
\vec v(0) = (1, -1)\ \mathrm{m/s}, \quad \vec r(0) = (0,0)\ \mathrm{m}.
$$

Determine:

1. Acceleration $\vec a(t)$
2. Velocity $\vec v(t)$
3. Position $\vec r(t)$
4. Trajectory of motion
5. Work done by the force at $t = 3\ \mathrm{s}$
6. Verification of the work-energy theorem

## Theory

For a constant force:

* Newton’s second law:

$$
\vec F = m \vec a \quad \Rightarrow \quad \vec a = \frac{\vec F}{m}
$$

* Velocity as a function of time:

$$
\vec v(t) = \vec v_0 + \vec a t
$$

* Position as a function of time:

$$
\vec r(t) = \vec r_0 + \int_0^t \vec v(\tau) d\tau = \vec r_0 + \vec v_0 t + \frac{1}{2} \vec a t^2
$$

* Work done by a constant force over displacement $\vec r(t)$:

$$
W(t) = \vec F \cdot (\vec r(t) - \vec r_0)
$$

* Kinetic energy:

$$
K(t) = \frac{1}{2} m |\vec v(t)|^2
$$

The **work-energy theorem** states:

$$
W = \Delta K = K(t) - K(0)
$$

## Step-by-Step Solution

### Step 1 – Compute acceleration

$$
\vec a = \frac{\vec F}{m} = \frac{[6, 2]}{2} = [3, 1] \ \mathrm{m/s^2}
$$

### Step 2 – Compute velocity

Velocity is linear in time:

$$
\vec v(t) = \vec v_0 + \vec a t = [1, -1] + [3, 1] t
$$

Component-wise:

$$
v_x(t) = 1 + 3t
$$

$$
v_y(t) = -1 + 1 \cdot t = -1 + t
$$

Thus:

$$
\vec v(t) = [1 + 3t, -1 + t] \ \mathrm{m/s}
$$

### Step 3 – Compute position

Position as a function of time:

$$
\vec r(t) = \vec r_0 + \vec v_0 t + \frac{1}{2} \vec a t^2
$$

Component-wise:

$$
x(t) = 0 + 1 \cdot t + \frac{1}{2} 3 t^2 = t + \frac{3 t^2}{2}
$$

$$
y(t) = 0 + (-1) \cdot t + \frac{1}{2} 1 \cdot t^2 = -t + \frac{t^2}{2}
$$

So:

$$
\vec r(t) = \left[ t + \frac{3 t^2}{2}, -t + \frac{t^2}{2} \right] \ \mathrm{m}
$$

### Step 4 – Trajectory

Eliminate $t$ to find $y(x)$:

From $x(t)$:

$$
x = t + \frac{3 t^2}{2} \quad \Rightarrow \quad 3 t^2 + 2 t - 2x = 0
$$

Solve for $t$:

$$
t = \frac{-2 + \sqrt{4 + 24 x}}{6} = \frac{-2 + \sqrt{4 + 24 x}}{6} \quad (\text{choose positive root})
$$

Then:

$$
y = -t + \frac{t^2}{2}
$$

This defines the **trajectory implicitly**. The motion is **parabolic**.

### Step 5 – Work done at $t = 3\ \mathrm{s}$

Displacement:

$$
\vec r(3) - \vec r_0 = \vec r(3) = \left[ 3 + \frac{3 \cdot 9}{2}, -3 + \frac{9}{2} \right] = [3 + 13.5, -3 + 4.5] = [16.5, 1.5] \ \mathrm{m}
$$

Work:

$$
W = \vec F \cdot (\vec r(3) - \vec r_0) = [6,2] \cdot [16.5, 1.5] = 6 \cdot 16.5 + 2 \cdot 1.5
$$

$$
W = 99 + 3 = 102\ \mathrm{J}
$$

### Step 6 – Check work-energy theorem

Kinetic energy at $t=0$:

$$
K_0 = \frac{1}{2} m |\vec v_0|^2 = \frac{1}{2} \cdot 2 \cdot (1^2 + (-1)^2) = 1 \cdot 2 = 2\ \mathrm{J}
$$

Velocity at $t=3$ s:

$$
\vec v(3) = [1 + 3 \cdot 3, -1 + 3] = [10, 2] \ \mathrm{m/s}
$$

Kinetic energy at $t=3$ s:

$$
K_3 = \frac{1}{2} m |\vec v(3)|^2 = 1 \cdot (10^2 + 2^2) = 1 \cdot (100 + 4) = 104\ \mathrm{J}
$$

Change in kinetic energy:

$$
\Delta K = K_3 - K_0 = 104 - 2 = 102\ \mathrm{J} = W
$$

 Verified. Work-energy theorem holds.

## Final Result

### Acceleration

$$
\vec a = [3, 1]\ \mathrm{m/s^2}
$$

### Velocity

$$
\vec v(t) = [1 + 3t, -1 + t]\ \mathrm{m/s}
$$

### Position

$$
\vec r(t) = \left[ t + \frac{3 t^2}{2}, -t + \frac{t^2}{2} \right]\ \mathrm{m}
$$

### Work done at $t=3$ s

$$
W = 102\ \mathrm{J}
$$

### Trajectory

Implicit form:

$$
y = -t + \frac{t^2}{2}, \quad x = t + \frac{3 t^2}{2}
$$

or parametric:

$$
x(t) = t + \frac{3 t^2}{2}, \quad y(t) = -t + \frac{t^2}{2}
$$

### Verification

Work-energy theorem holds:

$$
W = \Delta K = 102\ \mathrm{J}
$$

---
