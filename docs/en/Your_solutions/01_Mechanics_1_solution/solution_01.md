# Task 01 – Projectile Motion

## Problem Statement

A projectile is launched from the ground with initial velocity $v_0 = 100 \text{ m/s}$ at an angle $\theta = 37^\circ$. Air resistance is neglected.

Required:

* Differential equations of motion
* Time of flight
* Maximum height
* Range

---

## Theory

The motion is separated into two independent directions:

* Horizontal motion → constant velocity
* Vertical motion → constant acceleration due to gravity

Velocity components:

$$
v_{0x} = v_0 \cos\theta
$$

$$
v_{0y} = v_0 \sin\theta
$$

Acceleration:

$$
a_x = 0
$$

$$
a_y = -g
$$

---

## Step-by-Step Solution

### 1. Differential Equations of Motion

Horizontal motion:

$$
\frac{d^2 x}{dt^2} = 0
$$

This indicates constant velocity.

Vertical motion:

$$
\frac{d^2 y}{dt^2} = -g
$$

This indicates uniform downward acceleration.

---

### 2. Velocity Equations

Integrating acceleration:

Horizontal velocity:

$$
\frac{dx}{dt} = v_0 \cos\theta
$$

Vertical velocity:

$$
\frac{dy}{dt} = v_0 \sin\theta - gt
$$

---

### 3. Position Equations

Integrating velocity:

Horizontal position:

$$
x(t) = v_0 \cos\theta \cdot t
$$

Vertical position:

$$
y(t) = v_0 \sin\theta \cdot t - \frac{1}{2} g t^2
$$

---

### 4. Time of Flight

At landing:

$$
y(t) = 0
$$

Substitute:

$$
v_0 \sin\theta \cdot t - \frac{1}{2} g t^2 = 0
$$

Factor:

$$
t \left( v_0 \sin\theta - \frac{1}{2} g t \right) = 0
$$

Non-zero solution:

$$
t = \frac{2 v_0 \sin\theta}{g}
$$

Substitute values:

$$
t = \frac{2 \cdot 100 \cdot 0.6}{9.81}
$$

$$
t \approx 12.23 \text{ s}
$$

---

### 5. Maximum Height

At the top:

$$
v_y = 0
$$

From velocity equation:

$$
0 = v_0 \sin\theta - gt
$$

$$
t = \frac{v_0 \sin\theta}{g}
$$

Substitute into height equation:

$$
H = \frac{(v_0 \sin\theta)^2}{2g}
$$

$$
H = \frac{(100 \cdot 0.6)^2}{2 \cdot 9.81}
$$

$$
H \approx 183.49 \text{ m}
$$

---

### 6. Range

Range is horizontal distance:

$$
R = v_0 \cos\theta \cdot t
$$

Substitute $t$:

$$
R = \frac{v_0^2 \sin 2\theta}{g}
$$

$$
R = \frac{100^2 \cdot 0.96}{9.81}
$$

$$
R \approx 978.59 \text{ m}
$$

---

## Final Result

$$
T \approx 12.23 \text{ s}
$$

$$
H \approx 183.49 \text{ m}
$$

$$
R \approx 978.59 \text{ m}
$$

---

## Interpretation

* Horizontal motion remains constant because no force acts in that direction.
* Vertical motion changes due to gravity.
* The trajectory is parabolic.
* The angle $37^\circ$ gives a large range, close to the maximum possible value.
