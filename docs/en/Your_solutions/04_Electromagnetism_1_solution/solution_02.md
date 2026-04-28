# Section 4: Electromagnetism I - Problem 2

## 2. Electric Potential: Scalar Superposition in a Discrete System

**Problem:** Point charges of $+1\text{C}, -2\text{C}, +3\text{C},$ and $-4\text{C}$ are placed at the corners of a square with sides of $1.0 \text{ m}$ (in order). Calculate the electric potential at the center of the square.

---

### I. Geometric Parameters
In a square with side length $a = 1.0 \text{ m}$, all four corners are equidistant from the geometric center. This distance ($r$) is half of the diagonal:
$$d = a\sqrt{2} \implies r = \frac{a\sqrt{2}}{2}$$
For $a = 1.0 \text{ m}$:
$$r = \frac{\sqrt{2}}{2} \approx 0.707 \text{ m}$$

### II. Physical Principles
The **Electric Potential ($V$)** at a point due to a system of point charges is the algebraic sum of the potentials created by each charge. Unlike electric force or field, potential is a **scalar** quantity, meaning we do not use vector addition, only simple arithmetic summation.

The formula for the potential from a single point charge is:
$$V = k \frac{q}{r}$$
Where:
* $k \approx 8.99 \times 10^9 \text{ N}\cdot\text{m}^2/\text{C}^2$ (Coulomb's constant)
* $q$ is the charge (including its sign)
* $r$ is the distance from the charge to the point of interest

### III. Calculation Process
The total potential $V_{total}$ at the center is:
$$V_{total} = V_1 + V_2 + V_3 + V_4 = \sum \frac{k q_i}{r}$$

Since $r$ is common for all charges, we can factor out $k/r$:
$$V_{total} = \frac{k}{r} (q_1 + q_2 + q_3 + q_4)$$

Substituting the given charge values ($+1\text{C}, -2\text{C}, +3\text{C}, -4\text{C}$):
$$V_{total} = \frac{k}{r} (1 - 2 + 3 - 4)$$
$$V_{total} = \frac{k}{r} (-2)$$

### IV. Numerical Evaluation
Now, substitute the values for $k$ and $r$:
$$V_{total} = \frac{8.99 \times 10^9}{\sqrt{2}/2} \cdot (-2)$$
$$V_{total} = \frac{17.98 \times 10^9}{\sqrt{2}/2} \cdot (-1)$$
$$V_{total} = -2 \cdot \sqrt{2} \cdot (8.99 \times 10^9)$$
$$V_{total} \approx -2.54 \times 10^{10} \text{ V}$$

---

### Final Result
The electric potential at the center of the square is:
**$V \approx -2.54 \times 10^{10} \text{ Volts}$**

**Key Insight:** Even though the charges are arranged symmetrically, the potential is non-zero because the sum of the magnitudes of the charges is not zero. The negative result indicates that work must be done by an external agent to bring a positive test charge from infinity to this point.
