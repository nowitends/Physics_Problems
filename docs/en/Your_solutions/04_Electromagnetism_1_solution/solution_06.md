# Section 4: Electromagnetism I - Problem 6

## 6. Electric Field from a System of Point Charges

**Problem:** Two point charges are given: $+q$ at point $(-a, 0)$ and $+2q$ at point $(a, 0)$. 
1. Determine the field vectors $\vec{E}(0, y)$, $\vec{E}(x, 0)$, and the general field $\vec{E}(x, y)$.
2. Determine the conditions for which $E_x = 0, E_y = 0$, and the zero field point $\vec{E} = 0$.
3. Calculate the field for $a = 0.2 \text{ m}, y = 0.3 \text{ m}, q = 2 \mu\text{C}$ at $(0, y)$.
4. Investigate the limit $y \gg a$.

---

### I. General Field Vector $\vec{E}(x, y)$
Using the Principle of Superposition, the total field is the sum of the fields from $q_1$ ($+q$ at $-a$) and $q_2$ ($+2q$ at $+a$).
The displacement vectors from the charges to a point $P(x, y)$ are:
* $\vec{r}_1 = (x+a)\hat{i} + y\hat{j}$ with $r_1 = [(x+a)^2 + y^2]^{1/2}$
* $\vec{r}_2 = (x-a)\hat{i} + y\hat{j}$ with $r_2 = [(x-a)^2 + y^2]^{1/2}$

The general electric field is:
$$\vec{E}(x, y) = k q \left[ \frac{(x+a)\hat{i} + y\hat{j}}{((x+a)^2 + y^2)^{3/2}} + \frac{2(x-a)\hat{i} + 2y\hat{j}}{((x-a)^2 + y^2)^{3/2}} \right]$$

---

### II. Specific Field Vectors
**1. Field on the y-axis, $\vec{E}(0, y)$:**
Setting $x = 0$:
$$\vec{E}(0, y) = \frac{kq}{(a^2 + y^2)^{3/2}} \left[ (a\hat{i} + y\hat{j}) + 2(-a\hat{i} + y\hat{j}) \right]$$
$$\vec{E}(0, y) = \frac{kq}{(a^2 + y^2)^{3/2}} (-a\hat{i} + 3y\hat{j})$$

**2. Field on the x-axis, $\vec{E}(x, 0)$:**
Setting $y = 0$:
$$\vec{E}(x, 0) = kq \left[ \frac{(x+a)}{|x+a|^3}\hat{i} + \frac{2(x-a)}{|x-a|^3}\hat{i} \right]$$

---

### III. Equilibrium Conditions ($\vec{E} = 0$)
* **$E_y = 0$:** Occurs everywhere on the x-axis ($y=0$).
* **$E_x = 0$:** On the y-axis, $E_x$ is never zero (except at infinity) because the charges are unequal.
* **Zero Field Point:** Must lie on the x-axis between the charges ($-a < x < a$):
$$\frac{kq}{(x+a)^2} = \frac{k(2q)}{(a-x)^2} \implies (a-x)^2 = 2(x+a)^2$$
Taking the square root: $a-x = \sqrt{2}(x+a) \implies x = a \frac{1-\sqrt{2}}{1+\sqrt{2}} \approx -0.17a$

---

### IV. Numerical Calculation
**Given:** $a=0.2\text{ m}, y=0.3\text{ m}, q=2\times 10^{-6}\text{ C}$.
Distance $r = \sqrt{0.2^2 + 0.3^2} = \sqrt{0.13} \approx 0.36\text{ m}$.
Using $\vec{E}(0, y)$:
$$\vec{E} = \frac{(9\times 10^9)(2\times 10^{-6})}{(0.13)^{3/2}} (-0.2\hat{i} + 0.9\hat{j})$$
$$\vec{E} \approx 3.84 \times 10^5 (-0.2\hat{i} + 0.9\hat{j}) \text{ V/m}$$

---

### V. Limit Investigation ($y \gg a$)
As $y \to \infty$, $a$ becomes negligible ($r \approx y$):
$$\vec{E}(0, y) \approx \frac{kq}{y^3} (-a\hat{i} + 3y\hat{j}) \approx \frac{3kq}{y^2}\hat{j}$$
**Key Insight:** At great distances, the field approaches that of a single point charge with total magnitude $Q = q + 2q = 3q$.
