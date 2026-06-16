# Task 02 – Electric Potential at the Center of a Square

## Problem Statement

Point charges of $+1 , \text{C}$, $-2 , \text{C}$, $+3 , \text{C}$, and $-4 , \text{C}$ are placed at the corners of a square of side $1.0 , \text{m}$ (in order). Determine the electric potential at the center of the square.

---

## Theory

### Electric Potential Due to a Point Charge

The electric potential at a point due to a point charge is defined as

$$
V = k \frac{q}{r}
$$

where:

* $k = 9.0 \times 10^9 , \text{N m}^2/\text{C}^2$
* $q$ is the charge
* $r$ is the distance from the charge to the point

Electric potential represents the work done per unit charge in bringing a test charge from infinity to the point.

---

### Superposition Principle (Detailed Explanation)

The superposition principle states that when multiple charges are present, the total electric potential at a point is the algebraic sum of the potentials due to each individual charge.

Mathematically,

$$
V_{\text{net}} = V_1 + V_2 + V_3 + V_4 = k \left( \frac{q_1}{r_1} + \frac{q_2}{r_2} + \frac{q_3}{r_3} + \frac{q_4}{r_4} \right)
$$


---

## Step-by-Step Solution

### Step 1: Geometry of the Square

Side length:

$$
a = 1.0 , \text{m}
$$

Distance from center to each corner:

$$
r = \frac{a}{\sqrt{2}} = \frac{1}{\sqrt{2}} , \text{m}
$$

All four charges are at the same distance from the center.

---

### Step 2: Apply Superposition Principle

Since all distances are equal:

$$
V_{\text{net}} = k \cdot \frac{1}{r} (q_1 + q_2 + q_3 + q_4)
$$

Substitute the charges:

$$
q_{\text{total}} = 1 - 2 + 3 - 4
$$

$$
q_{\text{total}} = -2 , \text{C}
$$

---

### Step 3: Substitute Numerical Values

$$
V_{\text{net}} = 9.0 \times 10^9 \cdot \frac{-2}{\frac{1}{\sqrt{2}}}
$$

$$
V_{\text{net}} = 9.0 \times 10^9 \cdot (-2 \sqrt{2})
$$

$$
V_{\text{net}} = -18 \sqrt{2} \times 10^9
$$

---

### Step 4: Numerical Approximation

$$
\sqrt{2} \approx 1.414
$$

$$
V_{\text{net}} \approx -18 \times 1.414 \times 10^9
$$

$$
V_{\text{net}} \approx -25.45 \times 10^9 , \text{V}
$$

---

## Final Result

$$
V_{\text{center}} \approx -2.545 \times 10^{10} , \text{V}
$$

---

## Interpretation

The negative value of electric potential indicates that the overall influence of negative charges is stronger than that of positive charges.

Because electric potential is scalar:

* Contributions add directly without resolving directions
* Symmetry simplifies the calculation when distances are equal

The result represents the net work per unit charge required to bring a positive test charge from infinity to the center.
