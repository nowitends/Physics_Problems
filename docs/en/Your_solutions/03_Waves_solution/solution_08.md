# Task 08 – Waves

## Problem Statement

Determine which of the following functions satisfies the wave equation

$$
\frac{\partial^2 y}{\partial x^2} = \frac{1}{v^2} \frac{\partial^2 y}{\partial t^2}
$$

a) $y(x,t) = A \cos(kx^2 - \omega t)$

b) $y(x,t) = A(x - vt)^2$

c) $y(x,t) = A \log(x + vt)$

---

## Theory

A function represents a traveling wave if it satisfies the wave equation:

$$
\frac{\partial^2 y}{\partial x^2} = \frac{1}{v^2} \frac{\partial^2 y}{\partial t^2}
$$

A key result:

Any function of the form

$$
y(x,t) = f(x - vt) \quad \text{or} \quad f(x + vt)
$$

automatically satisfies the wave equation.

---

## Step-by-Step Solution

### a) $y(x,t) = A \cos(kx^2 - \omega t)$

Compute derivatives.

First derivative with respect to $x$:

$$
\frac{\partial y}{\partial x} = -A \sin(kx^2 - \omega t) \cdot (2kx)
$$

Second derivative:

$$
\frac{\partial^2 y}{\partial x^2} = -A \left[ \cos(kx^2 - \omega t)(2kx)^2 + \sin(kx^2 - \omega t)(2k) \right]
$$

This expression contains terms proportional to $x^2$ and constants.

Now differentiate with respect to $t$:

$$
\frac{\partial y}{\partial t} = A \sin(kx^2 - \omega t)\cdot \omega
$$

$$
\frac{\partial^2 y}{\partial t^2} = A \cos(kx^2 - \omega t)\cdot \omega^2
$$

The spatial derivative contains extra $x$-dependent terms that cannot match the time derivative form.

Therefore, the wave equation is not satisfied.

---

### b) $y(x,t) = A(x - vt)^2$

Let:

$$
u = x - vt
$$

Then:

$$
y = A u^2
$$

First derivatives:

$$
\frac{\partial y}{\partial x} = 2A u
$$

$$
\frac{\partial y}{\partial t} = 2A u(-v) = -2Avu
$$

Second derivatives:

$$
\frac{\partial^2 y}{\partial x^2} = 2A
$$

$$
\frac{\partial^2 y}{\partial t^2} = -2Av(-v) = 2Av^2
$$

Substitute into wave equation:

$$
\frac{1}{v^2} \frac{\partial^2 y}{\partial t^2} = \frac{1}{v^2}(2Av^2) = 2A
$$

Thus:

$$
\frac{\partial^2 y}{\partial x^2} = \frac{1}{v^2} \frac{\partial^2 y}{\partial t^2}
$$

The wave equation is satisfied.

---

### c) $y(x,t) = A \log(x + vt)$

Let:

$$
u = x + vt
$$

Then:

$$
y = A \log u
$$

First derivatives:

$$
\frac{\partial y}{\partial x} = \frac{A}{u}
$$

$$
\frac{\partial y}{\partial t} = \frac{A}{u} \cdot v
$$

Second derivatives:

$$
\frac{\partial^2 y}{\partial x^2} = -\frac{A}{u^2}
$$

$$
\frac{\partial^2 y}{\partial t^2} = -\frac{A v^2}{u^2}
$$

Substitute:

$$
\frac{1}{v^2} \frac{\partial^2 y}{\partial t^2} = \frac{1}{v^2} \left(-\frac{A v^2}{u^2}\right) = -\frac{A}{u^2}
$$

Thus:

$$
\frac{\partial^2 y}{\partial x^2} = \frac{1}{v^2} \frac{\partial^2 y}{\partial t^2}
$$

The wave equation is satisfied.

---

## Final Result

Valid traveling wave functions:

$$
\text{b) } y(x,t) = A(x - vt)^2
$$

$$
\text{c) } y(x,t) = A \log(x + vt)
$$

Invalid:

$$
\text{a) } y(x,t) = A \cos(kx^2 - \omega t)
$$

---

## Interpretation

* Functions of the form $f(x - vt)$ or $f(x + vt)$ always represent traveling waves.
* Options (b) and (c) follow this structure, so they satisfy the wave equation.
* Option (a) does not follow this form due to the nonlinear $x^2$ term, leading to mismatch in derivatives.
