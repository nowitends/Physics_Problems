# Solutions goes here

...
# Problem 1: Projectile Motion

**Problem Statement:**
A projectile is fired from the ground with an initial velocity of $v_0 = 100$ m/s at an angle of $\theta = 37^\circ$ above the horizontal. Assume no air resistance ($\sin 37^\circ \approx 0.6, \cos 37^\circ \approx 0.8, g = 9.81$ m/s²).

---

### a) Differential Equations of Motion
The motion is governed by gravity acting only in the vertical direction:
* **Horizontal direction ($x$):** $$\frac{d^2x}{dt^2} = 0$$
* **Vertical direction ($y$):** $$\frac{d^2y}{dt^2} = -g$$

### b) Time of Flight ($t_{total}$)
The time of flight is the total time until the projectile hits the ground ($y = 0$):
$$t = \frac{2 v_0 \sin \theta}{g} = \frac{2 \cdot 100 \cdot 0.6}{9.81} \approx \mathbf{12.23 \text{ s}}$$

### c) Maximum Height ($H$)
Maximum height is reached when the vertical velocity component becomes zero:
$$H = \frac{(v_0 \sin \theta)^2}{2g} = \frac{60^2}{2 \cdot 9.81} \approx \mathbf{183.48 \text{ m}}$$

### d) Range ($R$)
The total horizontal distance traveled is:
$$R = (v_0 \cos \theta) \cdot t = 80 \cdot 12.23 \approx \mathbf{978.4 \text{ m}}$$
