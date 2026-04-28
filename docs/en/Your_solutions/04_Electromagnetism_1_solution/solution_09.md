# Section 4: Electromagnetism I - Problem 9

## 9. Vector Lorentz Force: Cross Product Analysis

**Problem:** A proton moves with a velocity $\vec{v} = (2\hat{i} - 4\hat{j} + \hat{k}) \text{ m/s}$ in a region where the magnetic field is $\vec{B} = (\hat{i} + 2\hat{j} - \hat{k}) \text{ T}$. What is the magnitude of the magnetic force this charge experiences?

---

### I. Physical Principles
The magnetic force acting on a moving charge is defined by the vector cross product:
$$\vec{F} = q (\vec{v} \times \vec{B})$$

For a proton, the charge is $q = e \approx 1.6 \times 10^{-19} \text{ C}$.

### II. Calculating the Cross Product ($\vec{v} \times \vec{B}$)
The cross product is calculated using the determinant of a $3 \times 3$ matrix:
$$\vec{v} \times \vec{B} = \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ v_x & v_y & v_z \\ B_x & B_y & B_z \end{vmatrix} = \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ 2 & -4 & 1 \\ 1 & 2 & -1 \end{vmatrix}$$

**Expanding the determinant:**
* **$\hat{i}$ component:** $(-4)(-1) - (1)(2) = 4 - 2 = 2$
* **$\hat{j}$ component:** $-[(2)(-1) - (1)(1)] = -[-2 - 1] = 3$
* **$\hat{k}$ component:** $(2)(2) - (-4)(1) = 4 + 4 = 8$

Resulting vector:
$$\vec{v} \times \vec{B} = (2\hat{i} + 3\hat{j} + 8\hat{k})$$

### III. Calculating the Magnitude
First, find the magnitude of the cross product vector:
$$|\vec{v} \times \vec{B}| = \sqrt{(2)^2 + (3)^2 + (8)^2}$$
$$|\vec{v} \times \vec{B}| = \sqrt{4 + 9 + 64} = \sqrt{77} \approx 8.775 \text{ T}\cdot\text{m/s}$$

Now, multiply by the charge of the proton ($q = 1.6 \times 10^{-19} \text{ C}$):
$$F = q |\vec{v} \times \vec{B}| = (1.6 \times 10^{-19}) \cdot \sqrt{77}$$
$$F \approx 1.404 \times 10^{-18} \text{ N}$$

---

### Final Result
The magnitude of the magnetic force is:
**$F \approx 1.40 \times 10^{-18} \text{ N}$**

**Key Insight:** The force vector $\vec{F}$ is $1.6 \times 10^{-19} (2\hat{i} + 3\hat{j} + 8\hat{k}) \text{ N}$. This force is always perpendicular to both the velocity of the proton and the magnetic field lines.
