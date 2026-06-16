# Task 04 – Vector Calculus

## Problem Statement

The position of an object is given by

$$
\vec{r}(t) = (3t^2)\hat{i} + (5t - 8t^2)\hat{j}
$$

Determine:

* The velocity vector $\vec{v}(t)$
* The acceleration vector $\vec{a}(t)$

---

## Theory

* Velocity is the derivative of position with respect to time:

$$
\vec{v}(t) = \frac{d\vec{r}(t)}{dt}
$$

* Acceleration is the derivative of velocity with respect to time:

$$
\vec{a}(t) = \frac{d\vec{v}(t)}{dt}
$$

* Derivatives of powers of $t$:

$$
\frac{d}{dt}[t^n] = n t^{n-1}
$$

---

## Step-by-Step Solution

### 1. Position Components

Position vector:

$$
\vec{r}(t) = x(t) \hat{i} + y(t) \hat{j}
$$

with components:

$$
x(t) = 3t^2
$$

$$
y(t) = 5t - 8t^2
$$

---

### 2. Velocity Vector

Velocity is derivative of position:

$$
\vec{v}(t) = \frac{d}{dt}[x(t)] \hat{i} + \frac{d}{dt}[y(t)] \hat{j}
$$

Compute each component:

* $x$-component:

$$
v_x(t) = \frac{d}{dt}[3t^2] = 6t
$$

* $y$-component:

$$
v_y(t) = \frac{d}{dt}[5t - 8t^2] = 5 - 16t
$$

Thus:

$$
\vec{v}(t) = (6t)\hat{i} + (5 - 16t)\hat{j}
$$

---

### 3. Acceleration Vector

Acceleration is derivative of velocity:

$$
\vec{a}(t) = \frac{d}{dt}[v_x(t)] \hat{i} + \frac{d}{dt}[v_y(t)] \hat{j}
$$

Compute each component:

* $x$-component:

$$
a_x(t) = \frac{d}{dt}[6t] = 6
$$

* $y$-component:

$$
a_y(t) = \frac{d}{dt}[5 - 16t] = -16
$$

Thus:

$$
\vec{a}(t) = 6 \hat{i} - 16 \hat{j}
$$

---

## Final Result

Velocity vector:

$$
\vec{v}(t) = (6t)\hat{i} + (5 - 16t)\hat{j}
$$

Acceleration vector:

$$
\vec{a}(t) = 6 \hat{i} - 16 \hat{j}
$$

---

## Interpretation

* Velocity changes with time in both $x$ and $y$ directions
* Acceleration is constant in both directions
* The object is under uniform acceleration: $6 \text{ m/s}^2$ in $x$ and $-16 \text{ m/s}^2$ in $y$

The step-by-step derivative approach ensures understanding of how velocity and acceleration are obtained from position.
