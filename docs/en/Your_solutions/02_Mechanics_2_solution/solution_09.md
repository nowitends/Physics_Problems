# Task 09 – Vertical Throw with Linear Air Drag

## Problem Statement

A particle of mass $m$ is thrown vertically upward, experiencing linear air resistance. Its equation of motion is:

$$
m \frac{dv}{dt} = - m g - k v
$$

with initial conditions:

$$
v(0) = v_0, \quad x(0) = 10 \ \text{m}
$$

Tasks:

1. Solve the equation analytically for $v(t)$ and $x(t)$.
2. Determine the maximum height.
3. Compare with the case without drag.

---

## Theory

### Linear Air Resistance

The drag force is proportional to velocity:

$$
F_\text{drag} = - k v
$$

This is a common approximation for small velocities or low Reynolds numbers.

---

### Equation of Motion

Newton's second law:

$$
m \frac{dv}{dt} = - m g - k v
$$

Divide through by $m$:

$$
\frac{dv}{dt} + \frac{k}{m} v = - g
$$

This is a first-order linear ordinary differential equation (ODE) for $v(t)$.

---

### Work of Solving Linear ODE

For an equation of the form:

$$
\frac{dv}{dt} + p v = q
$$

The solution is:

$$
v(t) = e^{- \int p , dt} \left[ \int q e^{\int p , dt} dt + C \right]
$$

---

## Step-by-Step Solution

### Step 1: Solve for $v(t)$

The ODE:

$$
\frac{dv}{dt} + \frac{k}{m} v = - g
$$

Integrating factor:

$$
\mu(t) = e^{\int \frac{k}{m} dt} = e^{\frac{k}{m} t}
$$

Multiply both sides by $\mu(t)$:

$$
e^{\frac{k}{m} t} \frac{dv}{dt} + \frac{k}{m} e^{\frac{k}{m} t} v = - g e^{\frac{k}{m} t}
$$

Left-hand side is derivative of $v e^{\frac{k}{m} t}$:

$$
\frac{d}{dt} \left( v e^{\frac{k}{m} t} \right) = - g e^{\frac{k}{m} t}
$$

Integrate both sides:

$$
v e^{\frac{k}{m} t} = - g \int e^{\frac{k}{m} t} dt + C
$$

$$
v e^{\frac{k}{m} t} = - g \frac{m}{k} e^{\frac{k}{m} t} + C
$$

Solve for $v(t)$:

$$
v(t) = - \frac{m g}{k} + C e^{- \frac{k}{m} t}
$$

Apply initial condition $v(0) = v_0$:

$$
v_0 = - \frac{m g}{k} + C
$$

$$
C = v_0 + \frac{m g}{k}
$$

Thus:

$$
\boxed{v(t) = \left( v_0 + \frac{m g}{k} \right) e^{- \frac{k}{m} t} - \frac{m g}{k}}
$$

---

### Step 2: Solve for $x(t)$

Since $v = dx/dt$:

$$
dx/dt = \left( v_0 + \frac{m g}{k} \right) e^{- \frac{k}{m} t} - \frac{m g}{k}
$$

Integrate term by term:

$$
x(t) = \int \left( v_0 + \frac{m g}{k} \right) e^{- \frac{k}{m} t} dt - \int \frac{m g}{k} dt + x_0
$$

First integral:

$$
\int \left( v_0 + \frac{m g}{k} \right) e^{- \frac{k}{m} t} dt = - \frac{m}{k} \left( v_0 + \frac{m g}{k} \right) e^{- \frac{k}{m} t}
$$

Second integral:

$$
\int \frac{m g}{k} dt = \frac{m g}{k} t
$$

Combine with $x_0 = 10$ m:

$$
\boxed{x(t) = - \frac{m}{k} \left( v_0 + \frac{m g}{k} \right) e^{- \frac{k}{m} t} - \frac{m g}{k} t + \frac{m}{k} \left( v_0 + \frac{m g}{k} \right) + x_0}
$$

Simplify:

$$
x(t) = x_0 + \frac{m}{k} \left( v_0 + \frac{m g}{k} \right) \left( 1 - e^{- \frac{k}{m} t} \right) - \frac{m g}{k} t
$$

---

### Step 3: Maximum height

Maximum height occurs when $v(t) = 0$:

$$
0 = \left( v_0 + \frac{m g}{k} \right) e^{- \frac{k}{m} t_\text{max}} - \frac{m g}{k}
$$

Solve for $t_\text{max}$:

$$
\left( v_0 + \frac{m g}{k} \right) e^{- \frac{k}{m} t_\text{max}} = \frac{m g}{k}
$$

$$
e^{- \frac{k}{m} t_\text{max}} = \frac{\frac{m g}{k}}{v_0 + \frac{m g}{k}}
$$

$$

* \frac{k}{m} t_\text{max} = \ln \left( \frac{m g / k}{v_0 + m g / k} \right)
  $$

$$
t_\text{max} = - \frac{m}{k} \ln \left( \frac{m g}{k v_0 + m g} \right)
$$

Maximum height:

$$
x_\text{max} = x(t_\text{max})
$$

Substitute $t_\text{max}$ into $x(t)$:

$$
x_\text{max} = x_0 + \frac{m}{k} \left( v_0 + \frac{m g}{k} \right) \left[ 1 - \frac{m g / k}{v_0 + m g / k} \right] - \frac{m g}{k} t_\text{max}
$$

Simplify first bracket:

$$
1 - \frac{m g / k}{v_0 + m g / k} = \frac{v_0}{v_0 + m g / k}
$$

Hence:

$$
x_\text{max} = x_0 + \frac{m}{k} v_0 - \frac{m g}{k} t_\text{max}
$$

Substitute $t_\text{max}$:

$$
x_\text{max} = x_0 + \frac{m}{k} v_0 + \frac{m g}{k} \cdot \frac{m}{k} \ln \left( \frac{m g}{k v_0 + m g} \right)
$$

Or equivalently:

$$
x_\text{max} = x_0 + \frac{m v_0}{k} + \frac{m^2 g}{k^2} \ln \left( \frac{m g}{k v_0 + m g} \right)
$$

---

### Step 4: Comparison with no drag

Without drag ($k=0$), the equation reduces to standard vertical motion:

$$
v^2 = v_0^2 - 2 g (x - x_0)
$$

Maximum height:

$$
x_\text{max, no drag} = x_0 + \frac{v_0^2}{2 g}
$$

**Observation:** With drag, the maximum height is smaller because the drag force continuously dissipates energy.

---

## Final Result

**Velocity:**

$$
v(t) = \left( v_0 + \frac{m g}{k} \right) e^{- \frac{k}{m} t} - \frac{m g}{k}
$$

**Position:**

$$
x(t) = x_0 + \frac{m}{k} \left( v_0 + \frac{m g}{k} \right) \left( 1 - e^{- \frac{k}{m} t} \right) - \frac{m g}{k} t
$$

**Maximum height:**

$$
x_\text{max} = x_0 + \frac{m v_0}{k} + \frac{m^2 g}{k^2} \ln \left( \frac{m g}{k v_0 + m g} \right)
$$

---

## Interpretation

* Linear drag reduces the upward velocity exponentially.
* The particle reaches a lower maximum height than in the drag-free case.
* As $k \to 0$, the expressions reduce to standard free-flight motion with $x_\text{max} = x_0 + v_0^2 / (2g)$.
* The solution shows both exponential decay in velocity and the corresponding slowing of ascent due to energy loss to drag.
