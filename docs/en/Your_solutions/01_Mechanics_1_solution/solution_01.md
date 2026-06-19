# Problem 1: Projectile Motion

**Problem Statement:**
A projectile is fired from the ground with an initial velocity of $v_0 = 100$ m/s at an angle of $\theta = 37^\circ$ above the horizontal. Assume no air resistance ($\sin 37^\circ \approx 0.6$, $\cos 37^\circ \approx 0.8$, $g = 9.81$ m/s²).

---

### a) Differential Equations of Motion
In projectile motion, the only acceleration is gravity acting downwards.
* **Horizontal:** $a_x = \frac{d^2x}{dt^2} = 0$
* **Vertical:** $a_y = \frac{d^2y}{dt^2} = -g$

### b) Time of Flight ($t_{total}$)
The time of flight is found when the vertical displacement $y$ returns to zero:
$$t = \frac{2 v_0 \sin \theta}{g}$$
$$t = \frac{2 \cdot 100 \cdot 0.6}{9.81} \approx \mathbf{12.23 \text{ s}}$$

### c) Maximum Height ($H$)
Maximum height occurs when the vertical velocity $v_y = 0$:
$$H = \frac{(v_0 \sin \theta)^2}{2g}$$
$$H = \frac{(60)^2}{2 \cdot 9.81} \approx \mathbf{183.48 \text{ m}}$$

### d) Range ($R$)
The total horizontal distance traveled:
$$R = v_x \cdot t_{total} = (v_0 \cos \theta) \cdot t$$
$$R = 80 \cdot 12.23 \approx \mathbf{978.4 \text{ m}}$$
