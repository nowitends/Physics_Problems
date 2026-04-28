# Solution 1: Projectile Motion

## Problem Statement
A projectile is fired from the ground with:
- **Initial Velocity ($v_0$):** $100 \text{ m/s}$
- **Launch Angle ($\theta$):** $37^\circ$
- **Constants:** No air resistance, $g = 9.81 \text{ m/s}^2$
- **Approximations:** $\sin(37^\circ) \approx 0.6$, $\cos(37^\circ) \approx 0.8$

---

## 1. Differential Equations of Motion
In the absence of air resistance, the only force acting on the projectile is gravity in the vertical direction.

* **Horizontal (x-axis):** $$m \frac{d^2x}{dt^2} = 0 \implies \mathbf{\frac{d^2x}{dt^2} = 0}$$
* **Vertical (y-axis):** $$m \frac{d^2y}{dt^2} = -mg \implies \mathbf{\frac{d^2y}{dt^2} = -g}$$

---

## 2. Time of Flight ($t_{flight}$)
The projectile hits the ground when $y(t) = 0$. Using the equation $y(t) = (v_0 \sin\theta)t - \frac{1}{2}gt^2$:
$$t_{flight} = \frac{2v_0 \sin\theta}{g}$$
$$t_{flight} = \frac{2 \cdot 100 \cdot 0.6}{9.81} \approx \mathbf{12.23 \text{ s}}$$

---

## 3. Maximum Height ($H_{max}$)
The maximum height occurs when the vertical component of velocity is zero ($v_y = 0$):
$$H_{max} = \frac{(v_0 \sin\theta)^2}{2g}$$
$$H_{max} = \frac{(100 \cdot 0.6)^2}{2 \cdot 9.81} = \frac{3600}{19.62} \approx \mathbf{183.49 \text{ m}}$$

---

## 4. Range ($R$)
The horizontal distance covered during the entire flight time:
$$R = (v_0 \cos\theta) \cdot t_{flight}$$
$$R = (100 \cdot 0.8) \cdot 12.23 \approx \mathbf{978.4 \text{ m}}$$
