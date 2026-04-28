## 11. Dynamics with a Time-dependent Force

### Problem Statement
A particle of mass **$m = 3 \, kg$** moves in a force field $\vec{F}$ that depends on time as follows:
$$\vec{F}(t) = (15t, 3t - 12, -6t^2) \, \text{N}$$

Given the initial conditions at $t = 0$:
- Initial position: $\vec{r}_0 = (5, 2, -3) \, \text{m}$
- Initial velocity: $\vec{v}_0 = (2, 0, 1) \, \text{m/s}$

Find the time dependence of the particle's **velocity** $\vec{v}(t)$ and **position** $\vec{r}(t)$.

---

### Analytical Solution

#### Step 1: Find Acceleration $\vec{a}(t)$
Using Newton's Second Law ($\vec{a} = \vec{F}/m$):
$$\vec{a}(t) = \frac{1}{3} (15t, 3t - 12, -6t^2) = (5t, t - 4, -2t^2) \, \text{m/s}^2$$

#### Step 2: Find Velocity $\vec{v}(t)$
Velocity is the integral of acceleration with respect to time:
$$\vec{v}(t) = \int \vec{a}(t) \, dt + \vec{v}_0$$

- $v_x(t) = \int 5t \, dt + 2 = \frac{5}{2}t^2 + 2$
- $v_y(t) = \int (t - 4) \, dt + 0 = \frac{1}{2}t^2 - 4t$
- $v_z(t) = \int -2t^2 \, dt + 1 = -\frac{2}{3}t^3 + 1$

**Result:** $\vec{v}(t) = \left( \frac{5}{2}t^2 + 2, \frac{1}{2}t^2 - 4t, -\frac{2}{3}t^3 + 1 \right) \, \text{m/s}$

#### Step 3: Find Position $\vec{r}(t)$
Position is the integral of velocity with respect to time:
$$\vec{r}(t) = \int \vec{v}(t) \, dt + \vec{r}_0$$

- $x(t) = \int (\frac{5}{2}t^2 + 2) \, dt + 5 = \frac{5}{6}t^3 + 2t + 5$
- $y(t) = \int (\frac{1}{2}t^2 - 4t) \, dt + 2 = \frac{1}{6}t^3 - 2t^2 + 2$
- $z(t) = \int (-\frac{2}{3}t^3 + 1) \, dt - 3 = -\frac{1}{6}t^4 + t - 3$

**Result:** $\vec{r}(t) = \left( \frac{5}{6}t^3 + 2t + 5, \frac{1}{6}t^3 - 2t^2 + 2, -\frac{1}{6}t^4 + t - 3 \right) \, \text{m}$
