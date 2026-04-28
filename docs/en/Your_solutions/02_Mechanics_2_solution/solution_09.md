## 9. Vertical Throw with Drag (Differential Equations)

### Problem Statement
A particle of mass $m$ is thrown vertically with an initial velocity $v(0) = v_0$ from an initial height $x(0) = 10$. The equation of motion, including linear air drag, is given by:
$$m \frac{dv}{dt} = -mg - kv$$

1. Solve the equation analytically for velocity $v(t)$.
2. Determine the maximum height reached.
3. Compare the result with the ideal case (no air drag).
4. Outline a numerical simulation approach.

---

### Analytical Solution

#### 1. Solving for Velocity $v(t)$
We start by rearranging the equation into a first-order linear differential equation:
$$\frac{dv}{dt} + \frac{k}{m}v = -g$$

By using the integrating factor $e^{(k/m)t}$ or by separating the variables:
$$\int \frac{dv}{v + \frac{mg}{k}} = \int -\frac{k}{m} dt$$

After integrating and applying the initial condition $v(0) = v_0$, we get:
$$v(t) = \left( v_0 + \frac{mg}{k} \right) e^{-\frac{k}{m}t} - \frac{mg}{k}$$

#### 2. Maximum Height ($h_{max}$)
The particle reaches its maximum height when its velocity becomes zero ($v(t) = 0$).
Solving for time $t_{up}$:
$$0 = \left( v_0 + \frac{mg}{k} \right) e^{-\frac{k}{m}t_{up}} - \frac{mg}{k} \implies t_{up} = \frac{m}{k} \ln\left( 1 + \frac{kv_0}{mg} \right)$$

To find the height, we integrate $v(t)$ from $0$ to $t_{up}$ and add the initial height $x_0 = 10$.

#### 3. Comparison with Vacuum Case ($k=0$)
- **With Drag:** The particle experiences a greater downward acceleration during the ascent ($a = -g - \frac{kv}{m}$), resulting in a **lower maximum height** and a **shorter time to reach the peak** compared to the vacuum case.
- **Terminal Velocity:** As the particle falls back down, it will eventually reach a constant **terminal velocity** $v_t = -\frac{mg}{k}$, whereas in a vacuum, speed would increase indefinitely.

#### 4. Numerical Simulation (Python)
To visualize this motion, we can use the `odeint` solver from the `scipy` library:

```python
import numpy as np
from scipy.integrate import odeint

def drag_model(v, t, m, g, k):
    return -g - (k/m) * v

# Parameters: mass=3kg, g=9.81, k=0.1, v0=20m/s
t = np.linspace(0, 5, 100)
velocity = odeint(drag_model, 20.0, t, args=(3.0, 9.81, 0.1))
