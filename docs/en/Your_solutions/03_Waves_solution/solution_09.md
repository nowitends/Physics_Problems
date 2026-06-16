
---

# Task 09 – Damped Oscillator (Theory Notes)

## General Solution

The differential equation is

$$
m \frac{d^2 x}{dt^2} + b \frac{dx}{dt} + k x = 0
$$

Divide by $m$:

$$
\frac{d^2 x}{dt^2} + \frac{b}{m} \frac{dx}{dt} + \frac{k}{m} x = 0
$$

Characteristic equation:

$$
r^2 + \frac{b}{m} r + \frac{k}{m} = 0
$$

Solution:

$$
r = \frac{-b \pm \sqrt{b^2 - 4mk}}{2m}
$$

---

## Classification of Cases

### Underdamped ($b^2 < 4mk$)

$$
x(t) = A e^{-\frac{b}{2m}t} \cos(\omega_d t + \phi)
$$

where

$$
\omega_d = \sqrt{\frac{k}{m} - \left(\frac{b}{2m}\right)^2}
$$

---

### Critically Damped ($b^2 = 4mk$)

$$
x(t) = (A + Bt)e^{-\frac{b}{2m}t}
$$

---

### Overdamped ($b^2 > 4mk$)

$$
x(t) = A e^{r_1 t} + B e^{r_2 t}
$$

where $r_1, r_2$ are real and negative.

---

## Numerical Solution (RK4)

The second-order equation is rewritten as:

$$
\frac{dx}{dt} = v
$$

$$
\frac{dv}{dt} = -\frac{b}{m}v - \frac{k}{m}x
$$

These are solved using the **Runge–Kutta 4th order method**, implemented in the simulation.

---

## Interpretation

* Small $b$ → oscillations slowly decay (underdamped)
* Critical $b$ → fastest return to equilibrium without oscillation
* Large $b$ → slow return without oscillation (overdamped)

---

