# Task 06 – Variable Velocity

## Problem Statement

An object has velocity:

$$
v(t) = t^2 + 2t - 5
$$

Initial position:

$$
x(0) = 4
$$

Determine:

* Position $x(t)$ at $t = 3$
* Acceleration $a(t)$ at $t = 3$

---

## Theory

* Acceleration is the derivative of velocity:

$$
a(t) = \frac{dv}{dt}
$$

* Position is the integral of velocity:

$$
x(t) = x_0 + \int_0^t v(t) , dt
$$

* Step-by-step integration and differentiation provide the solution.

---

## Step-by-Step Solution

### 1. Acceleration

Velocity:

$$
v(t) = t^2 + 2t - 5
$$

Derivative gives acceleration:

$$
a(t) = \frac{d}{dt}[t^2 + 2t - 5]
$$

$$
a(t) = 2t + 2
$$

At $t = 3$:

$$
a(3) = 2(3) + 2 = 6 + 2 = 8
$$

---

### 2. Position

Position is integral of velocity:

$$
x(t) = x_0 + \int_0^t v(t) , dt
$$

$$
x(t) = 4 + \int_0^t (t^2 + 2t - 5) , dt
$$

Compute integral:

$$
\int (t^2 + 2t - 5) , dt = \frac{t^3}{3} + t^2 - 5t
$$

Add initial position:

$$
x(t) = 4 + \frac{t^3}{3} + t^2 - 5t
$$

At $t = 3$:

$$
x(3) = 4 + \frac{3^3}{3} + 3^2 - 5(3)
$$

Compute step-by-step:

$$
\frac{3^3}{3} = \frac{27}{3} = 9
$$

$$
3^2 = 9
$$

$$
-5(3) = -15
$$

Sum:

$$
x(3) = 4 + 9 + 9 - 15
$$

$$
x(3) = 7
$$

---

## Final Result

Position at $t = 3$:

$$
x(3) = 7
$$

Acceleration at $t = 3$:

$$
a(3) = 8
$$

---

## Interpretation

* The acceleration increases linearly with time: $a(t) = 2t + 2$
* The position grows according to the integral of velocity, showing non-uniform motion
* At $t = 3$, the object is at $x = 7$ and accelerating at $8 \text{ m/s}^2$
