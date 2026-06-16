# Task 03 – Proportionality in Universal Gravitation

## Problem Statement

The Universal Law of Gravitation is given by

$$
F = G \frac{m_1 m_2}{r^2}
$$

Determine how the gravitational force $F$ changes if:

* the distance $r$ is **doubled** ($r \to 2r$)
* both masses are **halved** ($m_1 \to \frac{m_1}{2}$, $m_2 \to \frac{m_2}{2}$)

---

## Theory

The **Universal Law of Gravitation** states that the gravitational force between two masses:

* is **directly proportional** to the product of the masses: $F \propto m_1 m_2$
* is **inversely proportional** to the square of the distance between them: $F \propto \frac{1}{r^2}$

Thus, any change in masses or distance will affect the force according to these proportionalities.

To find the **new force**, we can write

$$
F_{\text{new}} = G \frac{m_1' m_2'}{r'^2}
$$

Where $m_1'$, $m_2'$, and $r'$ are the changed values of the masses and distance.

The **factor of change** is then

$$
\text{Factor} = \frac{F_{\text{new}}}{F_{\text{original}}}
$$

This factor shows how many times larger or smaller the force becomes.

---

## Step-by-Step Solution

### Step 1 — Substitute the changed values

Halving the masses:

$$
m_1' = \frac{m_1}{2}, \quad m_2' = \frac{m_2}{2}
$$

Doubling the distance:

$$
r' = 2r
$$

Substitute these into the formula for the new force:

$$
F_{\text{new}} = G \frac{(\frac{m_1}{2})(\frac{m_2}{2})}{(2r)^2}
$$

---

### Step 2 — Simplify the numerator

$$
\frac{m_1}{2} \cdot \frac{m_2}{2} = \frac{m_1 m_2}{4}
$$

So

$$
F_{\text{new}} = G \frac{\frac{m_1 m_2}{4}}{(2r)^2}
$$

---

### Step 3 — Simplify the denominator

$$
(2r)^2 = 4 r^2
$$

Thus

$$
F_{\text{new}} = G \frac{\frac{m_1 m_2}{4}}{4 r^2}
$$

---

### Step 4 — Combine fractions

$$
F_{\text{new}} = G \frac{m_1 m_2}{16 r^2}
$$

---

### Step 5 — Express as a factor of the original force

The original force is

$$
F = G \frac{m_1 m_2}{r^2}
$$

Divide $F_{\text{new}}$ by $F$:

$$
\text{Factor} = \frac{F_{\text{new}}}{F} = \frac{G \frac{m_1 m_2}{16 r^2}}{G \frac{m_1 m_2}{r^2}} = \frac{1}{16}
$$

---

## Final Result

The gravitational force changes by a factor of

$$
\text{Factor} = \frac{1}{16}
$$

---

## Interpretation

After halving both masses and doubling the distance:

* The force becomes **16 times smaller** than the original force.
* This shows that distance has a strong effect on gravity due to the **inverse-square law**: doubling the distance reduces force by $4$ times, and halving each mass reduces the force by another factor of $4$.

In simple terms: **small masses and larger distances greatly reduce the gravitational pull**.
