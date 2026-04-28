## 1. Gravitational Dependence (Simple Pendulum)

### Problem Statement
1. A simple pendulum has a period of **4 seconds** on Earth. What would its period be on the Moon, where the gravitational acceleration is approximately $1/6$th of Earth's?
2. What is the required length $L$ of a simple pendulum to have a period of exactly **1 second** on Earth?

---

### Analytical Solution

The period $T$ of a simple pendulum is defined by the formula:
$$T = 2\pi\sqrt{\frac{L}{g}}$$

#### Part A: Period on the Moon
Given $T_{earth} = 4\,s$ and $g_{moon} = \frac{g_{earth}}{6}$. Since $T$ is inversely proportional to the square root of $g$ ($T \propto \frac{1}{\sqrt{g}}$):

$$\frac{T_{moon}}{T_{earth}} = \sqrt{\frac{g_{earth}}{g_{moon}}} = \sqrt{6}$$

Substituting the known values:
$$T_{moon} = 4 \times \sqrt{6}$$
$$T_{moon} \approx 4 \times 2.449 \approx \mathbf{9.80\,s}$$

**Conclusion:** The pendulum swings slower on the Moon due to weaker gravity.

#### Part B: Required Length on Earth
We want $T = 1.0\,s$ on Earth ($g \approx 9.81\,m/s^2$). We rearrange the period formula to solve for $L$:

$$L = \frac{T^2 \cdot g}{4\pi^2}$$

Substituting the values:
$$L = \frac{(1.0)^2 \cdot 9.81}{4 \cdot (3.14159)^2}$$
$$L = \frac{9.81}{39.478} \approx \mathbf{0.248\,m}$$

**Result:** The required length is approximately **24.8 cm**.
