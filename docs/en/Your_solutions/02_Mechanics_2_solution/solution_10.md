## 10. Force Field and Power (Kinematics & Dynamics)

### Problem Statement
In a certain force field, a particle with mass **$m = 0.5 \, kg$** moves according to the following position equations:
- $x(t) = 5t^2 - t$
- $y(t) = 2t^3$
- $z(t) = -3t + 2$

Find the time dependence of:
1. Velocity ($\vec{v}$)
2. Momentum ($\vec{p}$)
3. Acceleration ($\vec{a}$)
4. Force ($\vec{F}$)
5. Power ($P$) transferred by the field.

---

### Analytical Solution

#### 1. Velocity ($\vec{v}$)
Velocity is the first derivative of position with respect to time ($\vec{v} = \frac{d\vec{r}}{dt}$):
- $v_x = \frac{d}{dt}(5t^2 - t) = 10t - 1$
- $v_y = \frac{d}{dt}(2t^3) = 6t^2$
- $v_z = \frac{d}{dt}(-3t + 2) = -3$
**Result:** $\vec{v}(t) = (10t - 1) \hat{i} + 6t^2 \hat{j} - 3 \hat{k} \, \text{m/s}$

#### 2. Momentum ($\vec{p}$)
Momentum is defined as $\vec{p} = m\vec{v}$:
- $p_x = 0.5(10t - 1) = 5t - 0.5$
- $p_y = 0.5(6t^2) = 3t^2$
- $p_z = 0.5(-3) = -1.5$
**Result:** $\vec{p}(t) = (5t - 0.5) \hat{i} + 3t^2 \hat{j} - 1.5 \hat{k} \, \text{kg}\cdot\text{m/s}$

#### 3. Acceleration ($\vec{a}$)
Acceleration is the derivative of velocity ($\vec{a} = \frac{d\vec{v}}{dt}$):
- $a_x = \frac{d}{dt}(10t - 1) = 10$
- $a_y = \frac{d}{dt}(6t^2) = 12t$
- $a_z = \frac{d}{dt}(-3) = 0$
**Result:** $\vec{a}(t) = 10 \hat{i} + 12t \hat{j} + 0 \hat{k} \, \text{m/s}^2$

#### 4. Force ($\vec{F}$)
According to Newton's Second Law ($\vec{F} = m\vec{a}$):
- $F_x = 0.5(10) = 5$
- $F_y = 0.5(12t) = 6t$
- $F_z = 0.5(0) = 0$
**Result:** $\vec{F}(t) = 5 \hat{i} + 6t \hat{j} + 0 \hat{k} \, \text{N}$

#### 5. Power ($P$)
Power is the dot product of force and velocity ($P = \vec{F} \cdot \vec{v}$):
$$P(t) = F_x v_x + F_y v_y + F_z v_z$$
$$P(t) = 5(10t - 1) + 6t(6t^2) + 0(-3)$$
$$P(t) = 50t - 5 + 36t^3$$

**Result:** $P(t) = \mathbf{36t^3 + 50t - 5 \, \text{W}}$
