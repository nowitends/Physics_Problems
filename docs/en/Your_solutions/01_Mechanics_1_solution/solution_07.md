# Solution 7: Elimination of Time and Interpretation of Acceleration

## Problem Statement
The path of a particle is given by:
$$x(t) = 2t^2$$
$$y(t) = 3t^3$$

1. Eliminate the parameter $t$.
2. Calculate $\vec{v}(t)$, $|\vec{v}(t)|$, $\vec{a}(t)$, and $|\vec{a}(t)|$.
3. Determine if the acceleration is constant.

---

## 1. Eliminating the Parameter ($t$)
From the $x(t)$ equation:
$$x = 2t^2 \implies t^2 = \frac{x}{2} \implies t = \left(\frac{x}{2}\right)^{1/2}$$

Substitute $t$ into the $y(t)$ equation:
$$y = 3t^3 = 3 \left[\left(\frac{x}{2}\right)^{1/2}\right]^3$$
$$y = 3 \left(\frac{x}{2}\right)^{3/2} \quad \text{or} \quad \mathbf{y^2 = \frac{27}{8}x^3}$$

---

## 2. Velocity and Acceleration Vectors

### Velocity Vector ($\vec{v}$)
$$\vec{v}(t) = \frac{dx}{dt}\hat{i} + \frac{dy}{dt}\hat{j}$$
$$\vec{v}(t) = \mathbf{(4t)\hat{i} + (9t^2)\hat{j}}$$

**Magnitude of Velocity ($|\vec{v}|$):**
$$|\vec{v}(t)| = \sqrt{(4t)^2 + (9t^2)^2} = \mathbf{\sqrt{16t^2 + 81t^4}}$$

### Acceleration Vector ($\vec{a}$)
$$\vec{a}(t) = \frac{dv_x}{dt}\hat{i} + \frac{dv_y}{dt}\hat{j}$$
$$\vec{a}(t) = \mathbf{(4)\hat{i} + (18t)\hat{j}}$$

**Magnitude of Acceleration ($|\vec{a}|$):**
$$|\vec{a}(t)| = \sqrt{4^2 + (18t)^2} = \mathbf{\sqrt{16 + 324t^2}}$$

---

## 3. Is the Acceleration Constant?
The acceleration vector is $\vec{a}(t) = 4\hat{i} + 18t\hat{j}$. 

Because the y-component depends on time ($18t$), the acceleration vector changes as $t$ increases. 

**Conclusion:** No, the acceleration is **not constant**.

---

## 4. Trajectory Plot (Conceptual)
The trajectory follows a semi-cubical parabola shape ($y \propto x^{3/2}$), starting from the origin (0,0) and moving into the first quadrant as $t > 0$.
