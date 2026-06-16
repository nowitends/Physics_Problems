# Task 01 – Gravitational Dependence of a Simple Pendulum

## Problem Statement

A simple pendulum has a period of $4$ seconds on Earth. Determine its period on the Moon, where the gravitational acceleration is $\frac{1}{6}$ of that on Earth.

Additionally, determine the required length of a simple pendulum that has a period of exactly $1$ second on Earth.

## Theory

The period of a simple pendulum is given by

$$
T = 2\pi \sqrt{\frac{L}{g}}
$$

where:

* $T$ is the period,
* $L$ is the length of the pendulum,
* $g$ is the gravitational acceleration.

From this relation:

1. For constant length $L$, the period depends on gravity as

$$
T \propto \frac{1}{\sqrt{g}}
$$

2. Rearranging the formula to solve for $L$:

$$
L = \frac{g T^2}{4\pi^2}
$$

## Step-by-Step Solution

### Part A – Period on the Moon

Let:

* $T_E = 4 \text{ s}$ (Earth),
* $g_M = \frac{g_E}{6}$ (Moon).

Using the proportionality:

$$
\frac{T_M}{T_E} = \sqrt{\frac{g_E}{g_M}}
$$

Substituting $g_M = \frac{g_E}{6}$:

$$
\frac{T_M}{4} = \sqrt{\frac{g_E}{g_E/6}}
$$

$$
\frac{T_M}{4} = \sqrt{6}
$$

$$
T_M = 4\sqrt{6}
$$

Numerical value:

$$
T_M \approx 4 \times 2.45 = 9.8 \text{ s}
$$

### Part B – Required Length for $T = 1$ s

Using

$$
L = \frac{g T^2}{4\pi^2}
$$

Substitute:

* $g = 9.8 \text{ m/s}^2$,
* $T = 1 \text{ s}$

$$
L = \frac{9.8 \cdot (1)^2}{4\pi^2}
$$

$$
L = \frac{9.8}{4\pi^2}
$$

$$
L \approx \frac{9.8}{39.48} \approx 0.248 \text{ m}
$$

## Final Result

* Period on the Moon:

$$
T_M = 4\sqrt{6} \approx 9.8 \text{ s}
$$

* Required length for $T = 1$ s:

$$
L \approx 0.248 \text{ m}
$$

## Interpretation

The period of a pendulum increases when gravitational acceleration decreases. On the Moon, weaker gravity causes the pendulum to oscillate more slowly, increasing the period significantly.

A pendulum with a period of $1$ second on Earth must be relatively short (approximately $0.25$ m), showing that shorter lengths correspond to faster oscillations.
