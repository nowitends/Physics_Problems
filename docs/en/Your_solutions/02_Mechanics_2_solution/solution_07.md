## 7. Dynamics with Friction (Stacked Blocks)

### Problem Statement
A **5 kg** block ($m_1$) is placed on top of a **10 kg** block ($m_2$). 
- A horizontal force of **45 N** is applied to the 10 kg block.
- The 5 kg block is tied to a wall with a string, preventing it from moving.
- The coefficient of kinetic friction ($\mu_k$) between all surfaces is **0.2**.

Find the acceleration ($a$) of the 10 kg block. *(Using $g = 9.81 \, m/s^2$ for precision)*.

---

### Analytical Solution

To determine the acceleration, we analyze the forces acting specifically on the moving 10 kg block (Block 2).

#### Step 1: Friction between the two blocks ($f_1$)
As Block 2 moves, Block 1 (stationary) exerts a kinetic friction force on its top surface.
- **Normal Force ($N_1$):** $m_1 \cdot g = 5 \cdot 9.81 = 49.05 \, N$
- **Friction Force ($f_1$):** $\mu_k \cdot N_1 = 0.2 \cdot 49.05 = \mathbf{9.81 \, N}$

#### Step 2: Friction between the bottom block and the floor ($f_2$)
The floor must support the combined weight of both blocks.
- **Total Mass ($M$):** $m_1 + m_2 = 15 \, kg$
- **Normal Force ($N_2$):** $M \cdot g = 15 \cdot 9.81 = 147.15 \, N$
- **Friction Force ($f_2$):** $\mu_k \cdot N_2 = 0.2 \cdot 147.15 = \mathbf{29.43 \, N}$

#### Step 3: Calculation of Net Force ($F_{net}$)
The applied force ($F$) is opposed by both the upper friction ($f_1$) and the lower friction ($f_2$).
$$F_{net} = F_{applied} - f_1 - f_2$$
$$F_{net} = 45 - 9.81 - 29.43 = \mathbf{5.76 \, N}$$

#### Step 4: Newton's Second Law
Applying $F = m \cdot a$ to the 10 kg block ($m_2$):
$$a = \frac{F_{net}}{m_2} = \frac{5.76}{10} = \mathbf{0.576 \, m/s^2}$$

---

### Final Result
The acceleration of the 10 kg block is **$0.576 \, m/s^2$** (approximately **$0.58 \, m/s^2$**).

> **Key Takeaway:** Even though the top block is stationary, it still contributes to the total friction opposing the 45 N force.
