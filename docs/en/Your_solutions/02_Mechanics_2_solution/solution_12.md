## 12. Work and Energy with a Constant Force

### Problem Statement
A constant force acts on a body of mass **$m = 2 \, kg$**:
$$\vec{F} = (6, 2) \, \text{N}$$

The body starts from the origin $\vec{r}(0) = (0, 0)$ with an initial velocity:
$$\vec{v}(0) = (1, -1) \, \text{m/s}$$

Tasks:
1. Determine acceleration $\vec{a}(t)$, velocity $\vec{v}(t)$, and position $\vec{r}(t)$.
2. Calculate the work done by the force at time **$t = 3 \, s$**.
3. Verify the consistency with the **Work-Energy Theorem**.

---

### Analytical Solution

#### 1. Kinematics Equations
**Acceleration ($\vec{a}$):**
$$\vec{a} = \frac{\vec{F}}{m} = \frac{(6, 2)}{2} = \mathbf{(3, 1) \, m/s^2}$$

**Velocity ($\vec{v}(t)$):**
$$\vec{v}(t) = \int \vec{a} \, dt + \vec{v}_0 = (3t + 1, t - 1) \, \text{m/s}$$

**Position ($\vec{r}(t)$):**
$$\vec{r}(t) = \int \vec{v} \, dt + \vec{r}_0 = \left( \frac{3}{2}t^2 + t, \frac{1}{2}t^2 - t \right) \, \text{m}$$

#### 2. Work Done at $t = 3 \, s$
First, find the displacement $\Delta \vec{r}$ at $t = 3$:
- $x(3) = \frac{3}{2}(3)^2 + 3 = 13.5 + 3 = 16.5 \, m$
- $y(3) = \frac{1}{2}(3)^2 - 3 = 4.5 - 3 = 1.5 \, m$
- $\Delta \vec{r} = (16.5, 1.5) \, m$

Work is the dot product of force and displacement:
$$W = \vec{F} \cdot \Delta \vec{r} = (6)(16.5) + (2)(1.5)$$
$$W = 99 + 3 = \mathbf{102 \, J}$$

#### 3. Verification: Work-Energy Theorem
The theorem states $W = \Delta KE = KE_f - KE_i$.

**Initial Kinetic Energy ($KE_i$):**
$$v_i^2 = 1^2 + (-1)^2 = 2$$
$$KE_i = \frac{1}{2} m v_i^2 = \frac{1}{2}(2)(2) = 2 \, J$$

**Final Kinetic Energy ($KE_f$) at $t = 3$:**
- $\vec{v}(3) = (3(3)+1, 3-1) = (10, 2)$
- $v_f^2 = 10^2 + 2^2 = 104$
- $KE_f = \frac{1}{2} m v_f^2 = \frac{1}{2}(2)(104) = 104 \, J$

**Change in Kinetic Energy:**
$$\Delta KE = 104 - 2 = \mathbf{102 \, J}$$

**Conclusion:** Since $W = \Delta KE = 102 \, J$, the Work-Energy Theorem is verified.
