# Task 02 – Range Optimization

## Problem Statement

For projectile motion, the range is

$$
R(\theta) = \frac{v_0^2 \sin(2\theta)}{g}
$$

Show that the maximum range occurs at $\theta = 45^\circ$.

---

## Theory

* $v_0$ and $g$ are constants
* The only changing part is $\sin(2\theta)$
* The maximum value of $\sin(\text{anything})$ is $1$

---

## Step-by-Step Solution

### 1. Focus on the Important Part

$$
R(\theta) = \frac{v_0^2}{g} \sin(2\theta)
$$

The term $\frac{v_0^2}{g}$ is constant.

Thus, the range depends only on:

$$
\sin(2\theta)
$$

---

### 2. Maximum Value of Sine

The sine function satisfies:

$$
-1 \leq \sin(2\theta) \leq 1
$$

Maximum occurs when:

$$
\sin(2\theta) = 1
$$

---

### 3. Find the Angle

$$
\sin(2\theta) = 1
$$

This happens when:

$$
2\theta = 90^\circ
$$

Thus:

$$
\theta = 45^\circ
$$

---

### 4. Maximum Range

Substitute $\sin(2\theta) = 1$:

$$
R_{\text{max}} = \frac{v_0^2}{g}
$$

---

## Final Result

$$
\theta = 45^\circ
$$

$$
R_{\text{max}} = \frac{v_0^2}{g}
$$

---

## Interpretation

* The range depends only on $\sin(2\theta)$
* The sine function is largest at $90^\circ$
* This forces $2\theta = 90^\circ$
* Therefore, $\theta = 45^\circ$

At this angle, the projectile travels the maximum horizontal distance.
