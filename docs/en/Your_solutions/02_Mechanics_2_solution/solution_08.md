## 8. Work of a Variable Force (Conservative Fields)

### Problem Statement
Consider a one-dimensional conservative force given by:
$$F(x) = -kx$$
1. Write the equation of motion and solve it.
2. Calculate the work done by this force during a displacement from $x = 0$ to $x = x_0$.
3. Interpret the result in terms of potential energy ($U$).
4. Verify the relationship $F = -\frac{dU}{dx}$.
5. Describe the characteristic graphs of $F(x)$ and $U(x)$.

---

### Analytical Solution

#### 1. Equation of Motion
Using Newton's Second Law ($F = ma$):
$$m \frac{d^2x}{dt^2} = -kx \implies \frac{d^2x}{dt^2} + \frac{k}{m}x = 0$$
The general solution for this simple harmonic oscillator is:
$$x(t) = A \cos(\omega t + \phi), \quad \text{where } \omega = \sqrt{\frac{k}{m}}$$

#### 2. Work Done ($W$)
Since the force varies with position, we calculate work via integration:
$$W = \int_{0}^{x_0} F(x) \, dx = \int_{0}^{x_0} (-kx) \, dx$$
$$W = \left[ -\frac{1}{2}kx^2 \right]_{0}^{x_0} = \mathbf{-\frac{1}{2}kx_0^2}$$

#### 3. Potential Energy Interpretation
The work done by a conservative force is equal to the negative change in potential energy:
$$W = -\Delta U = -(U(x_0) - U(0))$$
If we set the reference point $U(0) = 0$, the potential energy stored at $x_0$ is:
$$U(x) = \frac{1}{2}kx^2$$

#### 4. Verification ($F = -dU/dx$)
Taking the negative derivative of the potential energy function:
$$-\frac{d}{dx} \left( \frac{1}{2}kx^2 \right) = -\left( \frac{1}{2} \cdot k \cdot 2x \right) = -kx$$
This matches our original force $F(x)$, confirming the force is conservative.

#### 5. Graphical Analysis
- **$F(x)$ vs $x$:** A linear graph with a negative slope ($-k$). It shows that the force always acts in the opposite direction of displacement (Restoring Force).
- **$U(x)$ vs $x$:** A parabolic curve opening upwards. The vertex at $(0,0)$ represents the stable equilibrium point where energy is at a minimum.

**Summary:** The negative work signifies that energy is being "stored" in the field as elastic potential energy.
