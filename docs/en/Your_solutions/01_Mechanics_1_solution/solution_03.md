# Solution 3: Path Intersection

## Problem Statement
Alice's path is given by: $A(t) = (2 + t, 8 - 3t)$
Bob's path is given by: $B(t) = (2t - 1, 2t + 2)$

We need to determine if they collide, if their paths intersect, or the minimum distance between them.

---

## 1. Checking for Collision
A collision occurs if $A(t) = B(t)$ for the same value of $t$.

**Step 1: Set the x-coordinates equal:**
$2 + t = 2t - 1$
$t = 3$

**Step 2: Check the y-coordinates at $t = 3$:**
$y_A(3) = 8 - 3(3) = 8 - 9 = -1$
$y_B(3) = 2(3) + 2 = 6 + 2 = 8$

Since $y_A(3) \neq y_B(3)$ ($-1 \neq 8$), **they do not collide.**

---

## 2. Checking for Path Intersection
An intersection occurs if they pass through the same point at *different* times ($t_1$ and $t_2$).

**Step 1: Set coordinates equal for different times:**
$x: 2 + t_1 = 2t_2 - 1 \implies t_1 = 2t_2 - 3$
$y: 8 - 3t_1 = 2t_2 + 2$

**Step 2: Substitute $t_1$ into the y-equation:**
$8 - 3(2t_2 - 3) = 2t_2 + 2$
$8 - 6t_2 + 9 = 2t_2 + 2$
$17 - 6t_2 = 2t_2 + 2$
$15 = 8t_2 \implies \mathbf{t_2 = 1.875}$
$\mathbf{t_1 = 2(1.875) - 3 = 0.75}$

**Conclusion:** Their paths **do intersect** at the point **(2.75, 5.75)**. However, Alice is there at $t = 0.75s$ and Bob is there at $t = 1.875s$.

---

## 3. Minimum Distance Calculation
Since they do not collide, we find the minimum distance $d(t)$ by minimizing the square of the distance function:
$f(t) = [x_B(t) - x_A(t)]^2 + [y_B(t) - y_A(t)]^2$
$f(t) = (t - 3)^2 + (5t - 6)^2$

**Step 1: Find the derivative $f'(t)$ and set to zero:**
$f'(t) = 2(t - 3) + 2(5t - 6)(5) = 0$
$2t - 6 + 50t - 60 = 0$
$52t = 66 \implies \mathbf{t \approx 1.27 \text{ s}}$

**Step 2: Calculate minimum distance at $t \approx 1.
