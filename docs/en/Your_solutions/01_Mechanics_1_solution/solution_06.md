## 6. Variable Velocity and Kinematics

### Problem Statement
An object's velocity is given by $v(t) = t^2 + 2t - 5$. If the object's position is $x = 4$ at $t = 0$, find its position and acceleration at $t = 3$.

---

### Solution

#### 1. Finding Acceleration ($a$)
Acceleration is the derivative of velocity with respect to time:
$$a(t) = \frac{dv}{dt} = \frac{d}{dt}(t^2 + 2t - 5) = 2t + 2$$
At $t = 3$:
$$a(3) = 2(3) + 2 = \mathbf{8\,m/s^2}$$

#### 2. Finding Position ($x$)
Position is the integral of velocity with respect to time:
$$x(t) = \int v(t) dt = \int (t^2 + 2t - 5) dt$$
$$x(t) = \frac{1}{3}t^3 + t^2 - 5t + C$$

Using the initial condition $x(0) = 4$:
$$4 = \frac{1}{3}(0)^3 + (0)^2 - 5(0) + C \implies C = 4$$
The position function is:
$$x(t) = \frac{1}{3}t^3 + t^2 - 5t + 4$$

At $t = 3$:
$$x(3) = \frac{1}{3}(3)^3 + (3)^2 - 5(3) + 4$$
$$x(3) = 9 + 9 - 15 + 4 = \mathbf{7}$$

---
**Result:** At $t = 3$, the acceleration is **$8\,m/s^2$** and the position is **$7$** units.
