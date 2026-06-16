# Task 06 – Function Analysis

## Problem Statement

Consider the function

$f(x) = 3x^2 - 12x + 7$

Determine whether the function has a **local maximum** or **local minimum**, and find the corresponding point.

---

## Theory

For a differentiable function $f(x)$:

1. **Critical points** occur where the first derivative equals zero.

$$
f'(x) = 0
$$

2. To determine the nature of the critical point, the **second derivative test** is used.

If

$$
f''(x) > 0
$$

the point is a **local minimum**.

If

$$
f''(x) < 0
$$

the point is a **local maximum**.

The coordinate of the extremum point is obtained by evaluating the function at the critical value.

$$
(x_c , f(x_c))
$$

---

## Step-by-Step Solution

### 1. Compute the First Derivative

Given

$$
f(x) = 3x^2 - 12x + 7
$$

Differentiate with respect to $x$.

$$
f'(x) = 6x - 12
$$

---

### 2. Find the Critical Point

Set the first derivative equal to zero.

$$
6x - 12 = 0
$$

Solve for $x$.

$$
6x = 12
$$

$$
x = 2
$$

Thus, the critical point occurs at

$$
x = 2
$$

---

### 3. Compute the Second Derivative

Differentiate the first derivative.

$$
f''(x) = 6
$$

---

### 4. Apply the Second Derivative Test

Evaluate the second derivative.

$$
f''(x) = 6 > 0
$$

Since the second derivative is positive, the function is **concave upward**, which indicates a **local minimum**.

---

### 5. Compute the Function Value at the Critical Point

Substitute $x = 2$ into the original function.

$$
f(2) = 3(2)^2 - 12(2) + 7
$$

$$
f(2) = 12 - 24 + 7
$$

$$
f(2) = -5
$$

---

## Final Result

The function has a **local minimum** at

$$
(2 , -5)
$$

---

## Interpretation

The quadratic function opens upward because the coefficient of $x^2$ is positive ($3 > 0$). Therefore, the parabola has a single lowest point.

The point

$$
(2 , -5)
$$

represents the **minimum value of the function**, meaning the function decreases until $x = 2$ and increases afterward.
