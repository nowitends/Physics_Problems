# Section 4: Electromagnetism I - Problem 3

## 3. Electrostatic Equilibrium: Finding the Zero-Force Point

**Problem:** Find the equilibrium position for a charge $q_3 = +1 \text{ C}$ placed on the line between a charge $q_1 = +4 \text{ C}$ and a charge $q_2 = +9 \text{ C}$, which are separated by a distance of $2 \text{ m}$.

---

### I. Physical Principles
For a point charge to be in **electrostatic equilibrium**, the net electric force acting on it must be zero ($\sum \vec{F} = 0$). 
* Since $q_1$ and $q_2$ are both positive, they will both exert repulsive forces on the positive charge $q_3$.
* For these forces to cancel each other out, $q_3$ must be placed somewhere on the line connecting $q_1$ and $q_2$, so that the forces act in opposite directions.

### II. Problem Setup
* Let the position of $q_1$ be at $x = 0$.
* Let the position of $q_2$ be at $x = 2.0 \text{ m}$.
* Let the position of $q_3$ be at a distance $x$ from $q_1$.
* Consequently, the distance from $q_3$ to $q_2$ is $(2.0 - x)$.

### III. Mathematical Derivation
Using **Coulomb's Law** ($F = k \frac{|q_a q_b|}{r^2}$), we set the magnitude of the force from $q_1$ equal to the magnitude of the force from $q_2$:

$$k \frac{q_1 q_3}{x^2} = k \frac{q_2 q_3}{(2.0 - x)^2}$$

We can simplify this equation by canceling the common terms $k$ and $q_3$:

$$\frac{4}{x^2} = \frac{9}{(2.0 - x)^2}$$

To solve for $x$ efficiently, we take the square root of both sides:

$$\sqrt{\frac{4}{x^2}} = \sqrt{\frac{9}{(2.0 - x)^2}} \implies \frac{2}{x} = \frac{3}{2.0 - x}$$

### IV. Solving for x
Cross-multiply to solve the linear equation:
$$2(2.0 - x) = 3x$$
$$4.0 - 2x = 3x$$
$$4.0 = 5x$$
$$x = \frac{4.0}{5} = 0.8 \text{ m}$$

---

### Final Result
The equilibrium position for $q_3$ is:
* **$0.8 \text{ m}$ from the $q_1 = +4 \text{ C}$ charge.**
* (Or $1.2 \text{ m}$ from the $q_2 = +9 \text{ C}$ charge).

**Key Insight:** The equilibrium point is closer to the smaller charge ($q_1$). This makes physical sense because a smaller charge requires a smaller distance to produce a force equal in magnitude to that of a larger charge.
