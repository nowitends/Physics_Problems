# Task 08 – Centripetal Acceleration at the Equator

## Problem Statement

Calculate the centripetal acceleration of a person standing on the Earth's equator. The given data is:

* Radius of the Earth: $R = 6378 \text{ km}$
* The Earth completes one rotation every $T = 24 \text{ hours}$

Determine the centripetal acceleration $a_c$.

## Theory

For an object moving in uniform circular motion, the centripetal acceleration is given by:

$$
a_c = \frac{v^2}{R}
$$

where $v$ is the linear speed of the object along the circular path of radius $R$.

The linear speed $v$ is related to the angular velocity $\omega$ by:

$$
v = \omega R
$$

The angular velocity of a rotating body is:

$$
\omega = \frac{2\pi}{T}
$$

where $T$ is the period of rotation.

Combining these, centripetal acceleration can also be written as:

$$
a_c = \omega^2 R
$$

## Step-by-Step Solution

**Step 1: Convert radius to meters**

$$
R = 6378 \text{ km} = 6378 \times 10^3 \text{ m} = 6.378 \times 10^6 \text{ m}
$$

**Step 2: Convert period to seconds**

$$
T = 24 \text{ hours} = 24 \times 3600 \text{ s} = 86400 \text{ s}
$$

**Step 3: Compute angular velocity**

$$
\omega = \frac{2\pi}{T} = \frac{2\pi}{86400} \text{ rad/s}
$$

$$
\omega \approx 7.2722 \times 10^{-5} \text{ rad/s}
$$

**Step 4: Compute centripetal acceleration**

$$
a_c = \omega^2 R
$$

$$
a_c = (7.2722 \times 10^{-5})^2 \times 6.378 \times 10^6
$$

$$
a_c \approx 0.0339 \text{ m/s}^2
$$

## Final Result

$$
a_c \approx 0.034 \text{ m/s}^2
$$

## Interpretation

The centripetal acceleration at the Earth's equator is very small compared to the acceleration due to gravity ($g \approx 9.81 \text{ m/s}^2$). This means that the effect of Earth's rotation slightly reduces the apparent weight of a person at the equator.
