# Task 03 – Path Intersection

## Problem Statement

Alice moves along:

$$
A(t) = (2 + t,; 8 - 3t)
$$

Bob moves along:

$$
B(t) = (2t - 1,; 2t + 2)
$$

Determine:

* Whether they intersect
* If not, find the minimum distance and when it occurs

---

## Theory

* Collision occurs if both $x$ and $y$ coordinates match at the same time
* If no collision, distance is:

$$
D(t) = \sqrt{(x_A - x_B)^2 + (y_A - y_B)^2}
$$

* Minimum distance occurs when:

$$
\frac{d}{dt} D^2(t) = 0
$$

---

## Step-by-Step Solution

### 1. Check for Intersection

Match $x$-coordinates:

$$
2 + t = 2t - 1
$$

$$
t = 3
$$

---

Check $y$ at $t = 3$:

Alice:

$$
y_A = 8 - 3(3) = -1
$$

Bob:

$$
y_B = 2(3) + 2 = 8
$$

Since:

$$
y_A \neq y_B
$$

No intersection occurs.

---

### 2. Form Distance Function

Difference in coordinates:

$$
x_A - x_B = (2 + t) - (2t - 1) = 3 - t
$$

$$
y_A - y_B = (8 - 3t) - (2t + 2) = 6 - 5t
$$

Distance:

$$
D(t) = \sqrt{(3 - t)^2 + (6 - 5t)^2}
$$

---

### 3. Square the Distance (to simplify)

$$
D^2(t) = (3 - t)^2 + (6 - 5t)^2
$$

Expand:

$$
(3 - t)^2 = t^2 - 6t + 9
$$

$$
(6 - 5t)^2 = 25t^2 - 60t + 36
$$

Add:

$$
D^2(t) = 26t^2 - 66t + 45
$$

---

### 4. Find Minimum Distance

Differentiate:

$$
\frac{d}{dt} D^2(t) = 52t - 66
$$

Set equal to zero:

$$
52t - 66 = 0
$$

$$
t = \frac{33}{26}
$$

---

### 5. Calculate Minimum Distance

Substitute $t = \frac{33}{26}$:

$$
D^2 = 26t^2 - 66t + 45
$$

$$
D^2 = 26\left(\frac{33}{26}\right)^2 - 66\left(\frac{33}{26}\right) + 45
$$

$$
D^2 \approx 3.11
$$

$$
D = \sqrt{3.11} \approx 1.77
$$

---

## Final Result

No intersection.

Time of closest approach:

$$
t = \frac{33}{26} \approx 1.27
$$

Minimum distance:

$$
D_{\min} \approx 1.77
$$

---

## Interpretation

* At $t = 3$, positions do not match → no collision
* Distance function is minimized using calculus
* The closest point occurs at $t \approx 1.27$
* Minimum separation between them is approximately $1.77$ units
