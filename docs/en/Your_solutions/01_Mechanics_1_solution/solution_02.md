## 2. Range Optimization (Analytical Proof)

### Problem Statement
Show that the maximum horizontal range $R$ for a projectile, given an initial velocity $v_0$, is achieved at a launch angle of $\theta = 45^\circ$.

---

### 1. Derivation of the Range Formula
To understand the optimization, we first define the horizontal ($x$) and vertical ($y$) positions:
* **Horizontal velocity:** $v_x = v_0 \cos\theta$
* **Vertical velocity:** $v_y = v_0 \sin\theta$

The time of flight ($t_f$) is found when the projectile hits the ground ($y = 0$):
$$y(t) = (v_0 \sin\theta)t - \frac{1}{2}gt^2 = 0 \implies t_f = \frac{2v_0 \sin\theta}{g}$$

The horizontal range $R$ is the distance traveled during this time:
$$R = v_x \cdot t_f = (v_0 \cos\theta) \left( \frac{2v_0 \sin\theta}{g} \right)$$
$$R = \frac{v_0^2}{g} (2 \sin\theta \cos\theta)$$

Using the trigonometric identity $2 \sin\theta \cos\theta = \sin(2\theta)$, we get:
$$R(\theta) = \frac{v_0^2 \sin(2\theta)}{g}$$

---

### 2. Finding the Maximum Range
To maximize $R(\theta)$, we take the derivative with respect to $\theta$ and set it to zero:
$$\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot \frac{d}{d\theta}[\sin(2\theta)] = 0$$

Applying the chain rule:
$$\frac{v_0^2}{g} \cdot 2\cos(2\theta) = 0$$

Since $\frac{2v_0^2}{g}$ is a constant and cannot be zero, we solve for:
$$\cos(2\theta) = 0$$

The cosine function is zero when the angle is $90^\circ$:
$$2\theta = 90^\circ \implies \mathbf{\theta = 45^\circ}$$

### 3. Conclusion
The maximum value of the sine function is $1$, which occurs when its argument is $90^\circ$. In the range formula, this corresponds to a launch angle of **$45^\circ$**. At this angle, the projectile achieves the optimal balance between air time and forward speed.
