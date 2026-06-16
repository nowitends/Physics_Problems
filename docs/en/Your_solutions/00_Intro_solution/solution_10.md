# Task 10 – Infinite Series: Ant’s Final Position

## Problem Statement

An ant starts at the origin $(0,0)$ and moves in the following repeating pattern:

* $1$ m **east**,
* $1/2$ m **north**,
* $1/3$ m **west**,
* $1/4$ m **south**,
* $1/5$ m **east**,
* $1/6$ m **north**, … and so on.

Determine the **final position** of the ant as it continues this movement indefinitely.

---

## Theory

The ant’s movement can be separated into **x-direction (east-west)** and **y-direction (north-south)** components.

* **East-West (x-axis):** Steps: $1$ m east, $1/3$ m west, $1/5$ m east, $1/7$ m west, …
* **North-South (y-axis):** Steps: $1/2$ m north, $1/4$ m south, $1/6$ m north, $1/8$ m south, …

The ant’s final position is obtained by **summing the infinite series** of x and y displacements separately.

---

## Step-by-Step Solution

### Step 1 – Separate x and y movements

**x-direction (east-west):**

$$
x_\text{total} = 1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \frac{1}{9} - \dots
$$

This is an **alternating series** of reciprocals of odd numbers.

**y-direction (north-south):**

$$
y_\text{total} = \frac{1}{2} - \frac{1}{4} + \frac{1}{6} - \frac{1}{8} + \dots
$$

This is an **alternating series** of reciprocals of even numbers.

---

### Step 2 – Recognize standard series

1. **x-direction series:**

$$
x_\text{total} = 1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \dots
$$

This is the **Gregory-Leibniz series** for $\pi$:

$$
1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \dots = \frac{\pi}{4}
$$

2. **y-direction series:**

Factor out $1/2$:

$$
y_\text{total} = \frac{1}{2}\left(1 - \frac{1}{2} + \frac{1}{3} - \frac{1}{4} + \dots\right)
$$

The series in parentheses is the **alternating harmonic series**, which converges to $\ln 2$:

$$
1 - \frac{1}{2} + \frac{1}{3} - \frac{1}{4} + \dots = \ln 2
$$

Therefore:

$$
y_\text{total} = \frac{1}{2} \ln 2
$$

---

### Step 3 – Write final position

The final position of the ant is:

$$
(x_\text{final}, y_\text{final}) = \left(\frac{\pi}{4}, \frac{\ln 2}{2}\right)
$$

---

## Final Result

$$
\text{Final position of the ant: } \left(\frac{\pi}{4}, \frac{\ln 2}{2}\right)
$$

---

## Interpretation

* The ant **never stops moving**, but the total distance in each direction converges to a finite value.
* The **x-coordinate** converges to $\pi/4$ meters (east), and the **y-coordinate** converges to $(\ln 2)/2$ meters (north).
* The ant’s final position is therefore **slightly east and slightly north of the origin**, at a precise point determined by these infinite series.
