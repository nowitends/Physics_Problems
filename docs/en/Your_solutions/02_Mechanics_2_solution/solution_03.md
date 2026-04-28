## 3. Conservation of Energy (Pendulum Velocity)

### Problem Statement
A pendulum with a length of **1.0 meter** is released from an initial angle of **$15^\circ$**. What is the speed of the pendulum bob at the bottom of its swing?
*(Assume $g = 9.81 \, m/s^2$)*

---

### Analytical Solution

In a closed system (ignoring air resistance), the mechanical energy is conserved. The potential energy at the release point is converted into kinetic energy at the lowest point.

#### Step 1: Find the Vertical Height ($h$)
When the pendulum is at an angle $\theta$, its height relative to the bottom is:
$$h = L - L \cos \theta = L(1 - \cos \theta)$$

Given:
- $L = 1.0 \, m$
- $\theta = 15^\circ$

$$h = 1.0 \times (1 - \cos 15^\circ)$$
Using $\cos 15^\circ \approx 0.9659$:
$$h = 1.0 \times (1 - 0.9659) = \mathbf{0.0341 \, m}$$

#### Step 2: Conservation of Energy
The potential energy ($PE$) at the top equals the kinetic energy ($KE$) at the bottom:
$$mgh = \frac{1}{2} m v^2$$

The mass $m$ cancels out, and we solve for $v$:
$$v = \sqrt{2gh}$$

#### Step 3: Final Calculation
Substituting the values:
$$v = \sqrt{2 \times 9.81 \times 0.0341}$$
$$v = \sqrt{0.669}$$
$$v \approx \mathbf{0.818 \, m/s}$$

**Result:** The speed of the pendulum bob at the bottom of the swing is approximately **0.82 m/s**.
