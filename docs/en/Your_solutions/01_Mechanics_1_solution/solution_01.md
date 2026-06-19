# Solutions goes here

# Mechanics and Kinematics: Analytical Solutions

This repository contains step-by-step analytical solutions to a comprehensive set of classical mechanics and kinematics problems.

## 1. Projectile Motion
---

A projectile is fired from the ground with an initial velocity of 100 m/s at an angle of 37° above the horizontal. Assume no air resistance.

**Solution:**

* **Differential equations of motion:**
    According to Newton's Second Law, the only force acting on the projectile after launch is gravity (assuming no air resistance).
    Horizontal (x-axis): $$m\ddot{x} = 0 \implies \ddot{x} = 0$$
    Vertical (y-axis): $$m\ddot{y} = -mg \implies \ddot{y} = -g$$

* **Time of flight ($T$):**
    The kinematic equation for vertical position is $y(t) = v_0 \sin(\theta)t - \frac{1}{2}gt^2$. Setting $y(T) = 0$:
    $$T = \frac{2v_0 \sin(\theta)}{g} \approx \frac{2(100)(0.60)}{9.8} \approx 12.24 \text{ s}$$

* **Maximum height ($H$):**
    Occurs when the vertical velocity $v_y = 0$, which happens at $t = \frac{T}{2}$:
    $$H = \frac{v_0^2 \sin^2(\theta)}{2g} \approx \frac{100^2 (0.60)^2}{2(9.8)} \approx 183.67 \text{ m}$$

* **Range ($R$):**
    The total horizontal distance traveled during the time of flight $T$:
    $$R = v_0 \cos(\theta) T = \frac{v_0^2 \sin(2\theta)}{g} \approx \frac{100^2 (0.96)}{9.8} \approx 979.59 \text{ m}$$


## 2. Range Optimization
---

For projectile motion, show analytically that the maximum range $R(\theta) = \frac{v_0^2 \sin(2\theta)}{g}$ for a given initial velocity is achieved at a launch angle of 45°.

**Solution:**

To find the angle $\theta$ that maximizes the range function $R(\theta)$, we take the first derivative with respect to $\theta$ and set it to zero:
$$\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot 2\cos(2\theta) = 0$$

Since $\frac{v_0^2}{g}$ is a non-zero constant, the equation is satisfied when:
$$\cos(2\theta) = 0 \implies 2\theta = 90^\circ \implies \theta = 45^\circ$$

To verify this is a maximum, the second derivative $\frac{d^2R}{d\theta^2} = -\frac{4v_0^2}{g}\sin(2\theta)$ is negative at $\theta = 45^\circ$.


## 3. Path Intersection
---

Alice is moving along a path described by $A(t) = (2+t, 8-3t)$ and Bob is moving along a path $B(t) = (2t-1, 2t+2)$. Determine if their paths intersect. If yes, determine when and where they will collide. If not, determine the minimum distance between them and when it occurs.

**Solution:**

* **Path Intersection:**
    We check if there is a spatial point $(x,y)$ they both cross, independent of time. Setting $A_x = B_x$ and $A_y = B_y$ for different times $t_A$ and $t_B$:
    1) $2 + t_A = 2t_B - 1 \implies t_A = 2t_B - 3$
    2) $8 - 3t_A = 2t_B + 2$
    
    Substituting (1) into (2) yields $t_B = 1.875 \text{ s}$ and $t_A = 0.75 \text{ s}$. The paths **do intersect** at $(2.75, 5.75)$.

* **Collision:**
    For a collision, they must be at the intersection point at the *same* time. Since $t_A \neq t_B$, they **do not collide**.

* **Minimum Distance:**
    The squared distance $D(t)^2$ between them at any time $t$ is:
    $$D(t)^2 = (x_A - x_B)^2 + (y_A - y_B)^2 = (3 - t)^2 + (6 - 5t)^2 = 26t^2 - 66t + 45$$
    Taking the derivative and setting it to zero:
    $$\frac{d(D^2)}{dt} = 52t - 66 = 0 \implies t = \frac{33}{26} \approx 1.27 \text{ s}$$
    Substituting $t$ back gives the minimum distance: $D_{min} = \frac{9}{\sqrt{26}} \approx 1.76 \text{ m}$.


## 4. Vector Calculus
---

The position of an object is given by $\vec{r}(t) = (3t^2)\hat{i} + (5t - 8t^2)\hat{j}$. Find the object's velocity and acceleration vectors as a function of time.

**Solution:**

* **Velocity:** First derivative of position with respect to time.
    $$\vec{v}(t) = \frac{d\vec{r}}{dt} = (6t)\hat{i} + (5 - 16t)\hat{j}$$
* **Acceleration:** Second derivative of position (or first derivative of velocity).
    $$\vec{a}(t) = \frac{d\vec{v}}{dt} = 6\hat{i} - 16\hat{j}$$


## 5. Relative Velocity
---

A river flows east at 2 m/s. A boat that can travel at 5 m/s in still water wants to go directly north across the river. In what direction (angle) should it head? How long will it take to cross the river if it's 200 meters wide?

**Solution:**

* **Heading:** To travel directly North, the boat's East/West velocity component must perfectly cancel the river's current. Let $\theta$ be the angle West of North:
    $$v_{boat}\sin(\theta) = v_{river} \implies 5\sin(\theta) = 2 \implies \sin(\theta) = 0.4$$
    $$\theta = \arcsin(0.4) \approx 23.58^\circ \text{ West of North}$$

* **Crossing Time:** The boat's effective speed North is $v_{y} = 5\cos(23.58^\circ) \approx 4.58 \text{ m/s}$. 
    $$t = \frac{Distance}{v_y} = \frac{200}{4.58} \approx 43.6 \text{ s}$$


## 6. Variable Velocity
---

An object's velocity is given by $v(t) = t^2 + 2t - 5$. If the object was at $x=4$ at $t=0$, what is its position and acceleration at time $t=3$?

**Solution:**

* **Position:** Integrate velocity. 
    $$x(t) = \int (t^2 + 2t - 5) dt = \frac{t^3}{3} + t^2 - 5t + C$$
    Using the initial condition $x(0) = 4 \implies C = 4$.
    At $t=3$: $x(3) = \frac{27}{3} + 9 - 15 + 4 = 7 \text{ m}$.

* **Acceleration:** Differentiate velocity.
    $$a(t) = \frac{dv}{dt} = 2t + 2$$
    At $t=3$: $a(3) = 2(3) + 2 = 8 \text{ m/s}^2$.


## 7. Elimination of Time and Acceleration
---

The path equation is given in parametric form: $x(t)=2t^2, \quad y(t)=3t^3$. Eliminate the parameter $t$. Calculate velocity, acceleration, and determine if acceleration is constant.

**Solution:**

* **Trajectory Equation (eliminating $t$):**
    From $x(t)$, we get $t = \sqrt{\frac{x}{2}}$ (assuming $t \ge 0$). Substituting this into $y(t)$:
    $$y(x) = 3\left(\sqrt{\frac{x}{2}}\right)^3 = \frac{3\sqrt{2}}{4}x^{3/2}$$

* **Velocity Vector and Magnitude:**
    $$\vec{v}(t) = \dot{x}\hat{i} + \dot{y}\hat{j} = 4t\hat{i} + 9t^2\hat{j}$$
    $$|\vec{v}(t)| = \sqrt{(4t)^2 + (9t^2)^2} = t\sqrt{16 + 81t^2}$$

* **Acceleration Vector and Magnitude:**
    $$\vec{a}(t) = \ddot{x}\hat{i} + \ddot{y}\hat{j} = 4\hat{i} + 18t\hat{j}$$
    $$|\vec{a}(t)| = \sqrt{16 + 324t^2} = 2\sqrt{4 + 81t^2}$$

* **Is acceleration constant?** No. Because the magnitude and the $\hat{j}$ component of $\vec{a}(t)$ depend on time $t$, the acceleration is variable.


## 8. Circular Motion
---

Calculate the centripetal acceleration of a person standing on the Earth's equator. The Earth's radius is approximately 6378 km.

**Solution:**

The Earth completes one rotation in $T \approx 24 \text{ hours} = 86,400 \text{ s}$. 
The angular velocity is $\omega = \frac{2\pi}{T}$. 
The centripetal acceleration is $a_c = \omega^2 R$:
$$a_c = \left(\frac{2\pi}{86400}\right)^2 (6,378,000 \text{ m}) \approx 0.0337 \text{ m/s}^2$$


## 9. Momentum Comparison
---

Which has greater momentum: a 2-gram fly flying at 10 m/s or a 60-gram tennis ball moving at 1 m/s?

**Solution:**

Momentum is defined as $p = mv$:
* **Fly:** $p = 0.002 \text{ kg} \times 10 \text{ m/s} = 0.02 \text{ kg}\cdot\text{m/s}$
* **Tennis Ball:** $p = 0.060 \text{ kg} \times 1 \text{ m/s} = 0.06 \text{ kg}\cdot\text{m/s}$

The **tennis ball** has a greater momentum.


## 10. 3D Kinematics
---

Point M moves according to the equation: $\vec{r}(t) = (a \cos(\omega t), b \sin(\omega t), bt)$ where $a, b, \omega$ are positive constants. Find the equation of the trajectory and compute the path length.

**Solution:**

* **Equation of the Trajectory:**
    Isolating trigonometric functions in the $x$ and $y$ components: $\frac{x}{a} = \cos(\omega t)$ and $\frac{y}{b} = \sin(\omega t)$. 
    Squaring and adding them yields the implicit equation:
    $$\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1$$
    This means the trajectory is an **elliptical helix** spiraling upwards along the surface of an elliptical cylinder.

* **Path Length ($s$):**
    First, find the velocity vector by taking the derivative of position: 
    $$\vec{v}(t) = (-a\omega \sin(\omega t), b\omega \cos(\omega t), b)$$
    The speed (magnitude of velocity) is:
    $$|\vec{v}(t)| = \sqrt{a^2\omega^2 \sin^2(\omega t) + b^2\omega^2 \cos^2(\omega t) + b^2}$$
    The path length from $t=0$ to $t=t_0$ is the integral of the speed:
    $$s = \int_0^{t_0} \sqrt{a^2\omega^2 \sin^2(\omega t) + b^2\omega^2 \cos^2(\omega t) + b^2} dt$$
    *(Note: If $a \neq b$, this requires an elliptic integral of the second kind. If $a = b$, it simplifies and can be integrated directly).*
