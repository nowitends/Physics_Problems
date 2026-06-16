# Task 08 – Area under the Curve of $f(x) = \sin(x)$

## Problem Statement

Calculate the area under the curve of the function

$$
f(x) = \sin(x)
$$

between $x = 0$ and $x = \pi$.

---

## Theory

The area under a curve $f(x)$ from $x = a$ to $x = b$ is given by the **definite integral**:

$$
\text{Area} = \int_a^b f(x) , dx
$$

For this problem:

* $f(x) = \sin(x)$
* Lower limit: $a = 0$
* Upper limit: $b = \pi$

The integral of $\sin(x)$ is:

$$
\int \sin(x) , dx = -\cos(x) + C
$$

where $C$ is the constant of integration. For a definite integral, $C$ cancels out.

---

## Step-by-Step Solution

### Step 1 – Write the definite integral

The area under the curve is:

$$
\text{Area} = \int_0^\pi \sin(x) , dx
$$

---

### Step 2 – Use the antiderivative of $\sin(x)$

The antiderivative of $\sin(x)$ is:

$$
\int \sin(x) , dx = -\cos(x)
$$

---

### Step 3 – Apply the limits of integration

Using the formula for definite integrals:

$$
\int_a^b f(x) , dx = F(b) - F(a)
$$

where $F(x)$ is the antiderivative. Substitute $F(x) = -\cos(x)$:

$$
\int_0^\pi \sin(x) , dx = \big[-\cos(x)\big]_0^\pi
$$

$$
\int_0^\pi \sin(x) , dx = \big[-\cos(\pi)\big] - \big[-\cos(0)\big]
$$

---

### Step 4 – Evaluate the cosine values

* $\cos(\pi) = -1$
* $\cos(0) = 1$

Substitute these values:

$$
\int_0^\pi \sin(x) , dx = [-(-1)] - [-(1)]
$$

$$
\int_0^\pi \sin(x) , dx = 1 - (-1)
$$

$$
\int_0^\pi \sin(x) , dx = 2
$$

---

## Final Result

$$
\text{Area under the curve} = 2
$$

---

## Interpretation

The area under the curve of $f(x) = \sin(x)$ from $x = 0$ to $x = \pi$ is $2$ square units. This corresponds to the positive "hump" of the sine function over one half-period.
