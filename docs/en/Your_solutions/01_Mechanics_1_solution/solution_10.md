# Task 10 – Kinematics of a Point

## Problem Statement

A point $M$ moves according to the parametric equation:

$$
\vec{r}(t) = (a \cos(\omega t), b \sin(\omega t), b t)
$$

where $a, b, \omega$ are positive constants.

Tasks:

a) Determine the equation of the point's trajectory.

b) Compute the path length of the point from $t = 0$ to $t = t_0$.

## Theory

1. **Trajectory equation**: The trajectory of a point is found by eliminating the time parameter $t$ from the parametric equations.

2. **Path length**: For a curve $\vec{r}(t) = (x(t), y(t), z(t))$, the path length $s$ from $t = 0$ to $t = t_0$ is:

$$
s = \int_0^{t_0} |\vec{v}(t)| , dt
$$

where $\vec{v}(t) = \frac{d\vec{r}}{dt}$ is the velocity vector.

## Step-by-Step Solution

### Part (a) – Equation of the trajectory

Given:

$$
x(t) = a \cos(\omega t), \quad y(t) = b \sin(\omega t), \quad z(t) = b t
$$

**Step 1: Eliminate $t$ from $x$ and $y$**

$$
\frac{x^2}{a^2} = \cos^2(\omega t), \quad \frac{y^2}{b^2} = \sin^2(\omega t)
$$

Add the equations:

$$
\frac{x^2}{a^2} + \frac{y^2}{b^2} = \cos^2(\omega t) + \sin^2(\omega t) = 1
$$

**Step 2: Include $z$**

From $z = b t$, the time parameter is:

$$
t = \frac{z}{b}
$$

Substitute into $x$ and $y$:

$$
x = a \cos\left(\omega \frac{z}{b}\right), \quad y = b \sin\left(\omega \frac{z}{b}\right)
$$

**Conclusion**: The trajectory is a **helix on an elliptical cylinder**.

### Part (b) – Path length from $t=0$ to $t=t_0$

**Step 1: Compute velocity vector**

$$
\vec{v}(t) = \frac{d\vec{r}}{dt} = (-a \omega \sin(\omega t), b \omega \cos(\omega t), b)
$$

**Step 2: Compute magnitude of velocity**

$$
|\vec{v}(t)| = \sqrt{(-a \omega \sin(\omega t))^2 + (b \omega \cos(\omega t))^2 + b^2}
$$

$$
|\vec{v}(t)| = \sqrt{a^2 \omega^2 \sin^2(\omega t) + b^2 \omega^2 \cos^2(\omega t) + b^2}
$$

Factor where possible:

$$
|\vec{v}(t)| = \sqrt{\omega^2 (a^2 \sin^2(\omega t) + b^2 \cos^2(\omega t)) + b^2}
$$

**Step 3: Path length integral**

$$
s = \int_0^{t_0} \sqrt{\omega^2 (a^2 \sin^2(\omega t) + b^2 \cos^2(\omega t)) + b^2} , dt
$$

This integral can be evaluated numerically for specific values of $a, b, \omega, t_0$.

## Final Result

**Trajectory equation**:

$$
\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1, \quad z \text{ free}
$$

**Path length**:

$$
s = \int_0^{t_0} \sqrt{\omega^2 (a^2 \sin^2(\omega t) + b^2 \cos^2(\omega t)) + b^2} , dt
$$

## Interpretation

The motion describes a **helix rising along $z$** while moving around an ellipse in the $xy$-plane. The velocity magnitude changes if $a \neq b$, reflecting the varying curvature of the elliptical path. The path length depends on both the rotation around the ellipse and the linear rise along $z$.
