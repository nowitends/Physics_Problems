# Task 09 – Optimization of Rectangle under a Curve

## Problem Statement

Determine the dimensions of a rectangle that lies under the curve

$$
y = 3 - x^2
$$

in the first quadrant ($x \ge 0$, $y \ge 0$), such that the rectangle has the **maximum area**.

---

## Theory

To maximize the area of a rectangle under a curve:

1. Let the **width** of the rectangle be $x$.
2. The **height** is given by the curve: $y = f(x) = 3 - x^2$.
3. The **area** of the rectangle is:

$$
A(x) = \text{width} \times \text{height} = x \cdot (3 - x^2)
$$

4. To find the **maximum area**, take the derivative of $A(x)$ and set it equal to zero:

$$
\frac{dA}{dx} = 0
$$

---

## Step-by-Step Solution

### Step 1 – Write the area formula

The rectangle has width $x$ and height $y = 3 - x^2$. So:

$$
A(x) = x \cdot (3 - x^2)
$$

Simplify:

$$
A(x) = 3x - x^3
$$

---

### Step 2 – Differentiate the area

Take derivative with respect to $x$:

$$
\frac{dA}{dx} = \frac{d}{dx}(3x - x^3)
$$

$$
\frac{dA}{dx} = 3 - 3x^2
$$

---

### Step 3 – Solve for $x$

Set derivative equal to zero:

$$
3 - 3x^2 = 0
$$

$$
x^2 = 1
$$

$$
x = 1
$$

(Only the positive value is used because $x \ge 0$.)

---

### Step 4 – Find height

Use $y = 3 - x^2$:

$$
y = 3 - 1^2
$$

$$
y = 2
$$

---

### Step 5 – Verify maximum

Second derivative:

$$
\frac{d^2A}{dx^2} = \frac{d}{dx}(3 - 3x^2) = -6x
$$

At $x = 1$:

$$
\frac{d^2A}{dx^2} = -6 < 0
$$

Negative value confirms **maximum**.

---

## Final Result

* **Width**: $x = 1$
* **Height**: $y = 2$
* **Maximum Area**:

$$
A_\text{max} = x \cdot y = 1 \cdot 2 = 2
$$

---

## Interpretation

The rectangle that fits under the curve in the first quadrant and has the largest area has **width = 1** and **height = 2**, giving a **maximum area of 2 square units**.

The top-right corner of the rectangle touches the curve $y = 3 - x^2$.
