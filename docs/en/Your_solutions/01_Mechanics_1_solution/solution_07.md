# Task 07 – Elimination of Time and Interpretation of Acceleration

## Problem Statement

The object moves along a parametric path:

$$
x(t) = 2t^2, \qquad y(t) = 3t^3
$$

Determine:

* The trajectory by eliminating the parameter $t$
* Draw the trajectory
* Velocity vector $\vec{v}(t)$ and its magnitude $|\vec{v}(t)|$
* Acceleration vector $\vec{a}(t)$ and its magnitude $|\vec{a}(t)|$
* Whether the acceleration is constant

---

## Theory

* **Eliminating the parameter**: Express $y$ directly as a function of $x$ by solving one equation for $t$ and substituting into the other.
* **Velocity vector**:

$$
\vec{v}(t) = \frac{dx}{dt} \hat{i} + \frac{dy}{dt} \hat{j}
$$

* **Speed**:

$$
|\vec{v}(t)| = \sqrt{v_x^2 + v_y^2}
$$

* **Acceleration vector**:

$$
\vec{a}(t) = \frac{d^2 x}{dt^2} \hat{i} + \frac{d^2 y}{dt^2} \hat{j}
$$

* **Acceleration magnitude**:

$$
|\vec{a}(t)| = \sqrt{a_x^2 + a_y^2}
$$

---

## Step-by-Step Solution

### 1. Eliminate Parameter $t$

From $x(t) = 2t^2$:

$$
t = \sqrt{\frac{x}{2}}
$$

Substitute into $y(t) = 3t^3$:

$$
y = 3 \left(\sqrt{\frac{x}{2}}\right)^3 = \frac{3}{2\sqrt{2}} x^{3/2}
$$

**Trajectory equation**:

$$
y = \frac{3}{2\sqrt{2}} x^{3/2}
$$

---

### 2. Draw the Trajectory

The trajectory $y = \frac{3}{2\sqrt{2}} x^{3/2}$ is **a curve starting at the origin and rising sharply**.

* For small $x$, $y$ grows slowly.
* For larger $x$, $y$ increases faster because of the $x^{3/2}$ term.
* This is a **non-linear curve in the first quadrant**.

Here is a rough plot of the trajectory:

```
y
|
|                *
|              *
|           *
|        *
|     *
|  *
|*
+------------------ x
```

* The curve **starts at (0,0)** and rises more steeply as $x$ increases.

---

### 3. Velocity Vector

$$
\frac{dx}{dt} = 4t, \qquad \frac{dy}{dt} = 9t^2
$$

$$
\vec{v}(t) = 4t \hat{i} + 9t^2 \hat{j}
$$

### 4. Speed

$$
|\vec{v}(t)| = \sqrt{(4t)^2 + (9t^2)^2} = t \sqrt{16 + 81 t^2}
$$

---

### 5. Acceleration Vector

$$
a_x = 4, \quad a_y = 18t
$$

$$
\vec{a}(t) = 4 \hat{i} + 18t \hat{j}
$$

### 6. Acceleration Magnitude

$$
|\vec{a}(t)| = \sqrt{16 + 324 t^2}
$$

* Depends on $t$, so acceleration is **not constant**

---

## Final Result

**Trajectory equation**:

$$
y = \frac{3}{2\sqrt{2}} x^{3/2}
$$

**Velocity vector**:

$$
\vec{v}(t) = 4t \hat{i} + 9t^2 \hat{j}
$$

**Speed**:

$$
|\vec{v}(t)| = t \sqrt{16 + 81 t^2}
$$

**Acceleration vector**:

$$
\vec{a}(t) = 4 \hat{i} + 18t \hat{j}
$$

**Acceleration magnitude**:

$$
|\vec{a}(t)| = \sqrt{16 + 324 t^2}
$$

**Acceleration constant?**

* No, it depends on $t$ → **not constant**

---

## Interpretation

* The path is a **non-linear curve** in the first quadrant, starting at the origin and rising more steeply as $x$ increases.
* Velocity grows in both $x$ and $y$ directions over time.
* Acceleration has a constant $x$ component and a $y$ component that increases linearly with time.
* Acceleration magnitude increases with time → **variable acceleration**.

---

