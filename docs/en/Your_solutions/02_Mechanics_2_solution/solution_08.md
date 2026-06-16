# Task 08 – Work of a Variable Force

## Problem Statement

A particle is subjected to a one-dimensional force:

$$
F(x) = - k x
$$

where $k > 0$ is a constant.

Tasks:

1. Write and solve the equation of motion.
2. Calculate the work done by the force during displacement from $x = 0$ to $x = x_0$.
3. Interpret the work as potential energy.
4. Verify the relation $F(x) = - \frac{dU}{dx}$.
5. Draw the graphs of $F(x)$ and $U(x)$.

---

## Theory

### Equation of Motion

Newton’s second law relates force to acceleration:

$$
F(x) = m \frac{d^2 x}{dt^2}
$$

Substituting the given force:

$$
m \frac{d^2 x}{dt^2} = - k x
$$

This is the standard equation of simple harmonic motion.

---

### Work Done by a Variable Force

Work done along a path from $x_1$ to $x_2$:

$$
W = \int_{x_1}^{x_2} F(x) , dx
$$

For conservative forces, the work can be interpreted as the negative change in potential energy:

$$
W = - \Delta U = U(x_1) - U(x_2)
$$

---

### Potential Energy

The potential energy function $U(x)$ satisfies:

$$
F(x) = - \frac{dU}{dx}
$$

---

## Step-by-Step Solution

### Step 1: Equation of motion

From Newton’s second law:

$$
m \frac{d^2 x}{dt^2} = - k x
$$

Rewriting:

$$
\frac{d^2 x}{dt^2} + \frac{k}{m} x = 0
$$

This is a second-order linear differential equation with constant coefficients.

---

### Step 2: General solution

The solution of:

$$
\frac{d^2 x}{dt^2} + \omega^2 x = 0, \quad \omega^2 = \frac{k}{m}
$$

is:

$$
x(t) = A \cos(\omega t) + B \sin(\omega t)
$$

where $A$ and $B$ are constants determined by initial conditions.

Velocity:

$$
v(t) = \frac{dx}{dt} = - A \omega \sin(\omega t) + B \omega \cos(\omega t)
$$

---

### Step 3: Work done from $0$ to $x_0$

The work done:

$$
W = \int_0^{x_0} F(x) , dx
$$

Substitute $F(x) = - k x$:

$$
W = \int_0^{x_0} (- k x) , dx
$$

$$
W = - k \int_0^{x_0} x , dx
$$

$$
W = - k \left[ \frac{x^2}{2} \right]_0^{x_0}
$$

$$
W = - \frac{1}{2} k x_0^2
$$

---

### Step 4: Potential energy interpretation

Potential energy is defined as:

$$
U(x) = - \text{Work done by conservative force from reference point to } x
$$

$$
U(x) = - W
$$

Thus:

$$
U(x) = \frac{1}{2} k x^2
$$

This shows that the work done by the force reduces the potential energy by:

$$
W = U(0) - U(x_0) = 0 - \frac{1}{2} k x_0^2 = - \frac{1}{2} k x_0^2
$$

---

### Step 5: Verify $F(x) = - \frac{dU}{dx}$

Compute derivative:

$$
\frac{dU}{dx} = \frac{d}{dx} \left( \frac{1}{2} k x^2 \right)
$$

$$
\frac{dU}{dx} = k x
$$

Hence:

$$
F(x) = - \frac{dU}{dx} = - k x
$$

This is consistent with the given force.

---

### Step 6: Graphs

* Force $F(x) = - k x$: linear function with negative slope, passing through origin.
* Potential energy $U(x) = \frac{1}{2} k x^2$: parabola opening upwards, minimum at $x=0$.

**Graphically:**

* $F(x)$: straight line through origin, negative slope.
* $U(x)$: parabola vertex at origin, symmetric about $x=0$.

---

## Final Result

**Equation of motion:**

$$
x(t) = A \cos(\omega t) + B \sin(\omega t), \quad \omega = \sqrt{\frac{k}{m}}
$$

**Work done from $0$ to $x_0$:**

$$
W = - \frac{1}{2} k x_0^2
$$

**Potential energy:**

$$
U(x) = \frac{1}{2} k x^2
$$

**Force verification:**

$$
F(x) = - \frac{dU}{dx} = - k x
$$

---

## Interpretation

* The particle undergoes simple harmonic motion about $x=0$.
* The work done by the restoring force reduces the particle’s potential energy.
* The potential energy function is quadratic in displacement, typical of linear restoring forces.
* The negative slope of $F(x)$ indicates that the force always acts opposite to displacement, consistent with a restoring force.
