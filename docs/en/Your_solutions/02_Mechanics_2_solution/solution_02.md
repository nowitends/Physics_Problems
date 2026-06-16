# Task 02 – Harmonic Motion

## Problem Statement

A mass of $10 , \text{kg}$ is attached to a spring and oscillates according to

$x(t) = 0.2 \cos(10\pi t)$

where $x$ is in meters and $t$ is in seconds.

Determine:

* the spring constant $k$,
* the total mechanical energy of the system.

## Theory

The general equation of simple harmonic motion is

$$
x(t) = A \cos(\omega t)
$$

where:

* $A$ is the amplitude,
* $\omega$ is the angular frequency.

For a mass–spring system, the angular frequency is related to the spring constant by

$$
\omega = \sqrt{\frac{k}{m}}
$$

Rewriting:

$$
k = m \omega^2
$$

The total mechanical energy in SHM is

$$
E = \frac{1}{2} k A^2
$$

## Step-by-Step Solution

### Step 1 – Identify parameters from the equation

Given:

$x(t) = 0.2 \cos(10\pi t)$

Thus:

* $A = 0.2 , \text{m}$
* $\omega = 10\pi , \text{rad/s}$
* $m = 10 , \text{kg}$

### Step 2 – Compute spring constant

Using

$$
k = m \omega^2
$$

Substitute values:

$$
k = 10 \cdot (10\pi)^2
$$

$$
k = 10 \cdot 100\pi^2
$$

$$
k = 1000\pi^2
$$

Numerical value:

$$
k \approx 1000 \times 9.87 \approx 9870 , \text{N/m}
$$

### Step 3 – Compute total mechanical energy

Using

$$
E = \frac{1}{2} k A^2
$$

Substitute values:

$$
E = \frac{1}{2} \cdot 1000\pi^2 \cdot (0.2)^2
$$

$$
E = \frac{1}{2} \cdot 1000\pi^2 \cdot 0.04
$$

$$
E = 20\pi^2
$$

Numerical value:

$$
E \approx 20 \times 9.87 \approx 197.4 , \text{J}
$$

## Final Result

Spring constant:

$$
k = 1000\pi^2 \approx 9870 , \text{N/m}
$$

Total mechanical energy:

$$
E = 20\pi^2 \approx 197.4,  \text{J}
$$

## Interpretation

The angular frequency determines the stiffness of the spring. A larger $\omega$ corresponds to a larger spring constant.

The total mechanical energy depends on the square of the amplitude, indicating that even small increases in amplitude significantly increase the stored energy.
