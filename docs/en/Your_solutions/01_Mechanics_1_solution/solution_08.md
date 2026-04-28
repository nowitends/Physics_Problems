# Solution 8: Circular Motion

## Problem Statement
Calculate the centripetal acceleration of a person standing on the Earth's equator.
- **Earth's Radius ($R$):** $6378 \text{ km} = 6.378 \times 10^6 \text{ m}$
- **Rotation Period ($T$):** 24 hours (1 sidereal day $\approx 86,400 \text{ s}$)

---

## 1. Relevant Formulas
The centripetal acceleration ($a_c$) can be calculated using the tangential velocity ($v$) or the angular velocity ($\omega$):
1. $\omega = \frac{2\pi}{T}$
2. $a_c = \omega^2 R$

---

## 2. Step-by-Step Calculation

### Step 1: Calculate Angular Velocity ($\omega$)
The Earth completes one full rotation ($2\pi$ radians) in 24 hours.
$$T = 24 \times 3600 = 86,400 \text{ s}$$
$$\omega = \frac{2\pi}{86,400} \approx 7.272 \times 10^{-5} \text{ rad/s}$$

### Step 2: Calculate Centripetal Acceleration ($a_c$)
Using the radius $R = 6,378,000 \text{ m}$:
$$a_c = \omega^2 \cdot R$$
$$a_c = (7.272 \times 10^{-5})^2 \cdot 6,378,000$$
$$a_c = (5.288 \times 10^{-9}) \cdot 6,378,000$$
$$a_c \approx \mathbf{0.0337 \text{ m/s}^2}$$

---

## 3. Conclusion
The centripetal acceleration of a person at the equator is approximately **$0.0337 \text{ m/s}^2$**.

*Note: This value is very small (about 0.34% of $g = 9.81 \text{ m/s}^2$), which is why we don't "feel" being thrown off the Earth, but it is enough to make the Earth slightly bulge at the equator.*
