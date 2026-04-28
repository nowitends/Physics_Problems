## 2. Harmonic Motion

### Problem Statement
A **10 kg** mass is attached to a spring and oscillates according to the displacement equation:
$$x(t) = 0.2 \cos(10\pi t)$$
*(where $x$ is in meters and $t$ is in seconds)*

Find the following:
1. The spring constant **$k$**.
2. The total mechanical energy **$E$** of the system.

---

### Analytical Solution

The general form of the displacement equation for Simple Harmonic Motion (SHM) is:
$$x(t) = A \cos(\omega t)$$

From the given equation, we identify the following parameters:
- **Amplitude ($A$):** $0.2 \, \text{m}$
- **Angular Frequency ($\omega$):** $10\pi \, \text{rad/s}$
- **Mass ($m$):** $10 \, \text{kg}$

#### Part A: Finding the Spring Constant ($k$)
The relationship between angular frequency, mass, and the spring constant is given by:
$$\omega = \sqrt{\frac{k}{m}} \implies \omega^2 = \frac{k}{m}$$

Solving for $k$:
$$k = m \cdot \omega^2$$
$$k = 10 \cdot (10\pi)^2 = 10 \cdot 100\pi^2 = 1000\pi^2$$
Using $\pi^2 \approx 9.87$:
$$k \approx \mathbf{9870 \, \text{N/m}}$$

#### Part B: Finding Total Mechanical Energy ($E$)
The total mechanical energy in a spring-mass system is the sum of kinetic and potential energy, which remains constant:
$$E_{total} = \frac{1}{2} k A^2$$

Substituting the values:
$$E = \frac{1}{2} \cdot (1000\pi^2) \cdot (0.2)^2$$
$$E = 500\pi^2 \cdot 0.04 = 20\pi^2$$
$$E \approx 20 \cdot 9.87 \approx \mathbf{197.4 \, \text{J}}$$

**Result:** The spring constant is approximately **9870 N/m** and the total energy is **197.4 Joules**.
