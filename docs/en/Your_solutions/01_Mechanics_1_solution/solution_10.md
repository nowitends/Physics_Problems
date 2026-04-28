# Solution 10: Kinematics (3D Motion)

## Problem Statement
A point $M$ moves according to the position vector:
$$\vec{r}(t) = (a \cos \omega t, b \sin \omega t, bt)$$
where $a, b, \omega$ are positive constants.

---

## a) Equation of the Trajectory
To find the trajectory in the $xy$-plane, we look at the first two components:
$x = a \cos(\omega t) \implies \frac{x}{a} = \cos(\omega t)$
$y = b \sin(\omega t) \implies \frac{y}{b} = \sin(\omega t)$

Using the identity $\cos^2\theta + \sin^2\theta = 1$:
$$\left(\frac{x}{a}\right)^2 + \left(\frac{y}{b}\right)^2 = 1$$

Since $z = bt$, the point moves upward at a constant rate while tracing an ellipse in the $xy$-plane.
**Conclusion:** The trajectory is an **Elliptical Helix**.

---

## b) Path Length from $t=0$ to $t=t_0$
Path length ($s$) is the integral of the magnitude of the velocity vector $|\vec{v}(t)|$:

1. **Velocity Vector:**
   $$\vec{v}(t) = \frac{d\vec{r}}{dt} = (-a\omega \sin \omega t, b\omega \cos \omega t, b)$$

2. **Magnitude $|\vec{v}(t)|$:**
   $$|\vec{v}(t)| = \sqrt{(-a\omega \sin \omega t)^2 + (b\omega \cos \omega t)^2 + b^2}$$
   $$|\vec{v}(t)| = \sqrt{a^2\omega^2 \sin^2 \omega t + b^2\omega^2 \cos^2 \omega t + b^2}$$

3. **Integral for Path Length:**
   $$s = \int_{0}^{t_0} \sqrt{a^2\omega^2 \sin^2 \omega t + b^2\omega^2 \cos^2 \omega t + b^2} \, dt$$
   *Note: If $a=b$, this
