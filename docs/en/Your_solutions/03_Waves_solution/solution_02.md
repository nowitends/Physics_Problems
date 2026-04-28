## 2. String Harmonics – Detailed Step-by-Step Solution

### **Problem Statement**
A guitar string is $64 \text{ cm}$ long and has a fundamental frequency (one antinode) of $330 \text{ Hz}$. What is the speed of the wave on this string?

---

### **Step 1: Physical Parameters & Unit Standardization**
To ensure the final speed is in meters per second ($\text{m/s}$), we must convert all units to the SI system:
* **Length ($L$):** $64 \text{ cm} = \mathbf{0.64 \text{ m}}$
* **Frequency ($f$):** $\mathbf{330 \text{ Hz}}$ (vibrations per second)
* **Harmonic State ($n$):** $1$ (Fundamental mode, meaning the simplest vibration pattern).

---

### **Step 2: Geometrical Derivation of Wavelength ($\lambda$)**
This is the most important step. A guitar string is fixed at both ends, creating **nodes** (points of zero displacement) at each bridge. 
* In the **fundamental frequency**, the string vibrates with exactly **one antinode** in the center.
* Geometrically, this vibration pattern represents exactly **one-half of a full sine wave**.

Therefore, the relationship between string length ($L$) and wavelength ($\lambda$) is:
$$L = \frac{1}{2} \lambda \implies \lambda = 2L$$

**Calculation of $\lambda$:**
$$\lambda = 2 \times 0.64 \text{ m}$$
$$\lambda = \mathbf{1.28 \text{ m}}$$
*(This $1.28 \text{ m}$ is the physical distance the wave would cover in one full cycle).*

---

### **Step 3: Calculating Wave Speed ($v$)**
Wave speed is defined as the product of how long each wave is ($\lambda$) and how many waves pass per second ($f$).

**The Calculation:**
$$v = f \cdot \lambda$$
$$v = 330 \text{ Hz} \times 1.28 \text{ m}$$

**Breaking down the multiplication:**
$$330 \times 1 = 330$$
$$330 \times 0.28 = 92.4$$
$$330 + 92.4 = \mathbf{422.4 \text{ m/s}}$$

---

### **Step 4: Summary of Results**
| Variable | Physical Meaning | Value |
| :--- | :--- | :--- |
| **$L$** | Physical string length | $0.64 \text{ m}$ |
| **$\lambda$** | Distance of one full oscillation | $1.28 \text{ m}$ |
| **$f$** | Rate of vibration | $330 \text{ Hz}$ |
| **$v$** | **Velocity of the wave on the string** | **$422.4 \text{ m/s}$** |

---

### **Step 5: Why is this speed so high? (Physical Insight)**
The value **$422.4 \text{ m/s}$** is faster than the speed of sound in air ($\approx 343 \text{ m/s}$). This is because:
1.  **Tension:** Guitar strings are under high tension.
2.  **Density:** The strings are relatively light (low linear mass density).
3.  **The Formula:** $v = \sqrt{\frac{T}{\mu}}$, where $T$ is tension and $\mu$ is mass per unit length. 

In this problem, we derived $v$ from the frequency and wavelength, which indirectly tells us that the tension and mass of this specific string are tuned to allow the wave to travel at exactly $422.4 \text{ m/s}$.
