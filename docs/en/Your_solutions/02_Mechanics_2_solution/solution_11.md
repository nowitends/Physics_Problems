# Task 11 – Dynamics with a Time-Dependent Force

## Problem Statement

A particle of mass $m=3$ kg moves in a force field

$$
F(t) = (15t, 3t-12, -6t^2) , \text{N}
$$

with initial conditions

$$
r_0 = (5,2,-3) , \text{m}, \quad v_0 = (2,0,1) , \text{m/s}.
$$

Determine the time dependence of the particle's **position** $r(t)$ and **velocity** $v(t)$.

## Theory

Newton's second law relates force and acceleration:

$$
F(t) = m a(t)
$$

or component-wise:

$$
a(t) = \frac{F(t)}{m}.
$$

Velocity is obtained by integrating acceleration:

$$
v(t) = v_0 + \int_0^t a(\tau) , d\tau.
$$

Position is obtained by integrating velocity:

$$
r(t) = r_0 + \int_0^t v(\tau) , d\tau.
$$

All operations are performed **component-wise**.

## Step-by-Step Solution

### Step 1 – Compute acceleration

Given $m=3$ kg, acceleration components are:

$$
a_x(t) = \frac{F_x}{m} = \frac{15t}{3} = 5t
$$

$$
a_y(t) = \frac{F_y}{m} = \frac{3t-12}{3} = t-4
$$

$$
a_z(t) = \frac{F_z}{m} = \frac{-6t^2}{3} = -2t^2
$$

Thus:

$$
a(t) = (5t, t-4, -2t^2)
$$

### Step 2 – Integrate acceleration to find velocity

Integrate each component from $0$ to $t$, adding initial velocity $v_0$:

$$
v_x(t) = v_{0x} + \int_0^t a_x(\tau) , d\tau = 2 + \int_0^t 5\tau , d\tau
$$

$$
v_x(t) = 2 + \left[ \frac{5 \tau^2}{2} \right]_0^t = 2 + \frac{5 t^2}{2}
$$

---

$$
v_y(t) = v_{0y} + \int_0^t a_y(\tau) , d\tau = 0 + \int_0^t (\tau-4) , d\tau
$$

$$
v_y(t) = \left[ \frac{\tau^2}{2} - 4\tau \right]_0^t = \frac{t^2}{2} - 4t
$$

---

$$
v_z(t) = v_{0z} + \int_0^t a_z(\tau) , d\tau = 1 + \int_0^t (-2\tau^2) , d\tau
$$

$$
v_z(t) = 1 + \left[ -\frac{2\tau^3}{3} \right]_0^t = 1 - \frac{2 t^3}{3}
$$

### Step 3 – Integrate velocity to find position

Integrate each component from $0$ to $t$, adding initial position $r_0$:

$$
x(t) = x_0 + \int_0^t v_x(\tau) , d\tau = 5 + \int_0^t \left( 2 + \frac{5 \tau^2}{2} \right) d\tau
$$

$$
x(t) = 5 + \left[ 2\tau + \frac{5 \tau^3}{6} \right]_0^t = 5 + 2t + \frac{5 t^3}{6}
$$

---

$$
y(t) = y_0 + \int_0^t v_y(\tau) , d\tau = 2 + \int_0^t \left( \frac{\tau^2}{2} - 4\tau \right) d\tau
$$

$$
y(t) = 2 + \left[ \frac{\tau^3}{6} - 2\tau^2 \right]_0^t = 2 + \frac{t^3}{6} - 2 t^2
$$

---

$$
z(t) = z_0 + \int_0^t v_z(\tau) , d\tau = -3 + \int_0^t \left( 1 - \frac{2 \tau^3}{3} \right) d\tau
$$

$$
z(t) = -3 + \left[ \tau - \frac{2 \tau^4}{12} \right]_0^t = -3 + t - \frac{t^4}{6}
$$

## Final Result

### Velocity

$$
v(t) =
\begin{pmatrix}
2 + \frac{5 t^2}{2} \
\frac{t^2}{2} - 4t \
1 - \frac{2 t^3}{3}
\end{pmatrix} \text{m/s}
$$

### Position

$$
r(t) =
\begin{pmatrix}
5 + 2t + \frac{5 t^3}{6} \
2 + \frac{t^3}{6} - 2 t^2 \
-3 + t - \frac{t^4}{6}
\end{pmatrix} \text{m}
$$

## Interpretation

* The particle experiences **quadratic acceleration** in $x$ and $z$, and **linear acceleration** in $y$.
* Velocity and position are **polynomial functions of time**, indicating non-uniform motion.
* The motion is three-dimensional, with each component evolving independently according to the force law.

---
