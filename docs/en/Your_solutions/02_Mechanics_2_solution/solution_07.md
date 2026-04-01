# Task 07 – Dynamics with Friction

## Problem Statement

A block of mass $m_1 = 5 \ \text{kg}$ is placed on top of a block of mass $m_2 = 10 \ \text{kg}$. A horizontal force $F = 45 \ \text{N}$ is applied to the $10 \ \text{kg}$ block. The $5 \ \text{kg}$ block is tied to a wall, so it remains stationary.

The coefficient of kinetic friction between all contacting surfaces is $\mu_k = 0.2$.

Determine the acceleration of the $10 \ \text{kg}$ block.

---

## Theory

### Kinetic Friction

The kinetic friction force is given by:

$$
f_k = \mu_k N
$$

where $N$ is the normal force between surfaces.

---

### Newton’s Second Law

The acceleration of a body is determined by the net force acting on it:

$$
\sum F = m a
$$

---

## Step-by-Step Solution

### Step 1: Forces acting on the 10 kg block

For the $10 \ \text{kg}$ block:

* Applied force $F = 45 \ \text{N}$ acts to the right
* Friction from the ground acts to the left
* Friction from the top block acts to the left

---

### Step 2: Normal force from the ground

The ground supports both masses:

$$
N_{\text{ground}} = (m_1 + m_2) g
$$

$$
N_{\text{ground}} = (5 + 10) \times 9.81
$$

$$
N_{\text{ground}} = 15 \times 9.81
$$

$$
N_{\text{ground}} = 147.15 \ \text{N}
$$

---

### Step 3: Friction between 10 kg block and ground

$$
f_{\text{ground}} = \mu_k N_{\text{ground}}
$$

$$
f_{\text{ground}} = 0.2 \times 147.15
$$

$$
f_{\text{ground}} = 29.43 \ \text{N}
$$

---

### Step 4: Friction between 5 kg and 10 kg block

Normal force between the blocks:

$$
N_{\text{top}} = m_1 g
$$

$$
N_{\text{top}} = 5 \times 9.81
$$

$$
N_{\text{top}} = 49.05 \ \text{N}
$$

Friction force:

$$
f_{\text{top}} = \mu_k N_{\text{top}}
$$

$$
f_{\text{top}} = 0.2 \times 49.05
$$

$$
f_{\text{top}} = 9.81 \ \text{N}
$$

---

### Step 5: Net force on the 10 kg block

Total opposing friction:

$$
f_{\text{total}} = f_{\text{ground}} + f_{\text{top}}
$$

$$
f_{\text{total}} = 29.43 + 9.81
$$

$$
f_{\text{total}} = 39.24 \ \text{N}
$$

Net force:

$$
F_{\text{net}} = 45 - 39.24
$$

$$
F_{\text{net}} = 5.76 \ \text{N}
$$

---

### Step 6: Acceleration

$$
a = \frac{F_{\text{net}}}{m_2}
$$

$$
a = \frac{5.76}{10}
$$

$$
a = 0.576 \ \text{m/s}^2
$$

---

## Final Result

$$
a = 0.576 \ \text{m/s}^2
$$

---

## Interpretation

The applied force must overcome two friction forces: one between the lower block and the ground, and another between the two blocks. Since the top block is fixed to the wall, relative motion occurs at the interface, producing kinetic friction.

The combined friction significantly reduces the net force, resulting in a relatively small acceleration of the $10 \ \text{kg}$ block.
