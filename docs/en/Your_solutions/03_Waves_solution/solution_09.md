## 9. Damped Oscillator

**Problem:**
A damped harmonic oscillator is governed by the differential equation:
$$m \frac{d^2x}{dt^2} + b \frac{dx}{dt} + kx = 0$$
where $m = 1 \text{ kg}$, $k = 5 \text{ N/m}$, and $b$ is the damping coefficient.
1. Solve for the position $x(t)$ given $x(0) = 1$ and $v(0) = 0$.
2. Explain the different damping regimes based on the value of $b$.

**Solution:**

The auxiliary equation for this differential equation is:
$$ms^2 + bs + k = 0$$

Using the quadratic formula, the roots are:
$$s = \frac{-b \pm \sqrt{b^2 - 4mk}}{2m}$$

The behavior of the system depends on the discriminant ($D = b^2 - 4mk$):

### 1. Underdamped ($b^2 < 20$)
If $b$ is small (e.g., $b=0.5$), the roots are complex. The solution takes the form:
$$x(t) = e^{-\gamma t} (A \cos(\omega_d t) + B \sin(\omega_d t))$$
where $\gamma = b/2m$ is the damping factor and $\omega_d$ is the damped natural frequency. The system oscillates with decaying amplitude.

### 2. Critically Damped ($b^2 = 20 \implies b \approx 4.47$)
The system returns to equilibrium as quickly as possible without oscillating. The solution is:
$$x(t) = (A + Bt)e^{-\gamma t}$$

### 3. Overdamped ($b^2 > 20$)
If $b$ is large (e.g., $b=10$), the roots are real and negative. The system returns to equilibrium slowly without any oscillation:
$$x(t) = Ae^{s_1 t} + Be^{s_2 t}$$

**Conclusion:** For the given parameters, the threshold between oscillating and not oscillating occurs at $b = \sqrt{20} \approx 4.47 \text{ kg/s}$.
