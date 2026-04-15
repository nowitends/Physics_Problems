# Task 06 – Electric Field Due to Two Charges

## Problem Statement

Two point charges are placed on the x-axis:

* $+q$ at $(-a, 0)$
* $+2q$ at $(a, 0)$

Tasks:

1. Determine $\vec E(0, y)$, $\vec E(x, 0)$, and general $\vec E(x, y)$
2. Find conditions for $E_x = 0$, $E_y = 0$, and $\vec E = 0$
3. Compute field for $a = 0.2,\text{m}$, $y = 0.3,\text{m}$, $q = 2,\mu\text{C}$
4. Investigate the limit $y \gg a$

---

## Theory

### Electric Field of a Point Charge

$$
\vec E = k \frac{q}{r^3} \vec r
$$

where:

* $\vec r = \text{position vector from charge to field point}$
* $r = |\vec r|$

---

## Step-by-Step Solution

## Part 1: General Field $\vec E(x,y)$

### Contribution from $+q$ at $(-a,0)$

Position vector:

$$
\vec r_1 = (x + a)\hat i + y \hat j
$$

Magnitude:

$$
r_1 = \sqrt{(x+a)^2 + y^2}
$$

Field:

$$
\vec E_1 = k \frac{q}{r_1^3} \left[(x+a)\hat i + y \hat j\right]
$$

---

### Contribution from $+2q$ at $(a,0)$

$$
\vec r_2 = (x - a)\hat i + y \hat j
$$

$$
r_2 = \sqrt{(x-a)^2 + y^2}
$$

$$
\vec E_2 = k \frac{2q}{r_2^3} \left[(x-a)\hat i + y \hat j\right]
$$

---

### Total Field

$$
\vec E(x,y) = \vec E_1 + \vec E_2
$$

$$
\vec E =
k \left[
\frac{q(x+a)}{r_1^3} + \frac{2q(x-a)}{r_2^3}
\right]\hat i
+
k \left[
\frac{qy}{r_1^3} + \frac{2qy}{r_2^3}
\right]\hat j
$$

---

## Part 2: Field on Axes

### (a) Field at $(0,y)$

Substitute $x=0$:

$$
r_1 = r_2 = \sqrt{a^2 + y^2}
$$

$x$-component:

$$
E_x = k \left[\frac{qa}{r^3} + \frac{2q(-a)}{r^3}\right]
$$

$$
E_x = k \frac{-qa}{r^3}
$$

$y$-component:

$$
E_y = k \left[\frac{qy}{r^3} + \frac{2qy}{r^3}\right]
$$

$$
E_y = k \frac{3qy}{r^3}
$$

---

### (b) Field at $(x,0)$

Set $y=0$:

$$
E_y = 0
$$

$$
E_x = k \left[
\frac{q(x+a)}{|x+a|^3} + \frac{2q(x-a)}{|x-a|^3}
\right]
$$

---

## Part 3: Conditions for Zero Components

### Condition for $E_y = 0$

From general expression:

$$
E_y = k y \left[\frac{q}{r_1^3} + \frac{2q}{r_2^3}\right]
$$

Thus:

$$
E_y = 0 \Rightarrow y = 0
$$

---

### Condition for $E_x = 0$ (on x-axis)

$$
\frac{q}{(x+a)^2} = \frac{2q}{(x-a)^2}
$$

Cancel $q$:

$$
\frac{1}{(x+a)^2} = \frac{2}{(x-a)^2}
$$

Solve:

$$
(x-a)^2 = 2(x+a)^2
$$

Take square root:

$$
x-a = \sqrt{2}(x+a)
$$

Solve:

$$
x - \sqrt{2}x = a(\sqrt{2} + 1)
$$

$$
x(1 - \sqrt{2}) = a(\sqrt{2} + 1)
$$

$$
x = \frac{a(\sqrt{2} + 1)}{1 - \sqrt{2}}
$$

---

### Condition for $\vec E = 0$

Requires both:

$$
E_x = 0 \quad \text{and} \quad E_y = 0
$$

Thus only possible on x-axis at the above $x$.

---

## Part 4: Numerical Calculation at $(0,y)$

Given:

* $a = 0.2$
* $y = 0.3$
* $q = 2 \times 10^{-6}$

Distance:

$$
r = \sqrt{0.2^2 + 0.3^2} = \sqrt{0.13} \approx 0.36
$$

---

### Compute Components

#### $E_x$

$$
E_x = -k \frac{qa}{r^3}
$$

$$
= -9 \times 10^9 \cdot \frac{(2 \times 10^{-6})(0.2)}{(0.36)^3}
$$

$$
E_x \approx -7.7 \times 10^4 , \text{N/C}
$$

---

#### $E_y$

$$
E_y = k \frac{3qy}{r^3}
$$

$$
= 9 \times 10^9 \cdot \frac{3(2 \times 10^{-6})(0.3)}{(0.36)^3}
$$

$$
E_y \approx 3.5 \times 10^5 , \text{N/C}
$$

---

## Part 5: Limit $y \gg a$

If $y \gg a$, then:

$$
r_1 \approx r_2 \approx y
$$

Thus:

$$
E_x \approx 0
$$

$$
E_y \approx k \frac{3q}{y^2}
$$

---

## Final Result

General field:

$$
\vec E =
k \left[
\frac{q(x+a)}{r_1^3} + \frac{2q(x-a)}{r_2^3}
\right]\hat i
+
k \left[
\frac{qy}{r_1^3} + \frac{2qy}{r_2^3}
\right]\hat j
$$

Numerical value at $(0,0.3)$:

$$
\vec E \approx (-7.7 \times 10^4)\hat i + (3.5 \times 10^5)\hat j
$$

---

## Interpretation

* The stronger charge ($2q$) dominates the horizontal component
* At large distances, the system behaves like a single charge $3q$
* The field becomes nearly vertical for $y \gg a$
* The zero-field point lies closer to the smaller charge due to imbalance in magnitudes
