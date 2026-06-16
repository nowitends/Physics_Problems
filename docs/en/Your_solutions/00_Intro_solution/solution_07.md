# Task 07 – Fly and Bicycle Problem (Direct Time-Based Approach)

## Problem Statement

A bicycle is initially located 10 meters from a wall and moves toward the wall at a constant speed of $1\text{ m/s}$. A fly starts at the front wheel of the bicycle and flies toward the wall at a constant speed of $2\text{ m/s}$. Upon reaching the wall, the fly instantly reverses direction and flies back toward the bicycle, continuing this back-and-forth motion until the bicycle collides with the wall. Determine the total distance traveled by the fly before being crushed.

---

## Theory

The fly moves continuously at a constant speed during the entire motion until the bicycle reaches the wall. The total distance traveled by the fly is therefore given by:

$$
d_\text{fly} = v_\text{fly} \cdot t_\text{collision}
$$

where:

* $v_\text{fly}$ is the constant speed of the fly.
* $t_\text{collision}$ is the time it takes for the bicycle to reach the wall.

This approach eliminates the need to calculate each leg of the fly’s back-and-forth motion.

---

## Step-by-Step Solution

### Step 1 – Calculate time for the bicycle to reach the wall

The bicycle travels at a constant speed $v_\text{bicycle} = 1\text{ m/s}$, and the initial distance to the wall is $x_0 = 10\text{ m}$. Using the formula for constant speed:

$$
t_\text{collision} = \frac{\text{distance}}{\text{speed}}
$$

Substitute the values:

$$
t_\text{collision} = \frac{10}{1}
$$

$$
t_\text{collision} = 10 \text{ s}
$$

---

### Step 2 – Calculate the total distance traveled by the fly

The fly moves at a constant speed $v_\text{fly} = 2\text{ m/s}$ during the time $t_\text{collision}$. Using the distance formula:

$$
d_\text{fly} = v_\text{fly} \cdot t_\text{collision}
$$

Substitute the values:

$$
d_\text{fly} = 2 \cdot 10
$$

$$
d_\text{fly} = 20 \text{ m}
$$

---

## Final Result

$$
\text{Total distance traveled by the fly} = 20 \text{ m}
$$

---

## Interpretation

The fly travels continuously at its constant speed until the bicycle hits the wall. The total distance depends only on the fly’s speed and the time until collision. The repeated back-and-forth motion does not change the result.
