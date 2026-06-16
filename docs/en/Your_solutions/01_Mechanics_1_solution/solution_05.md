# Task 05 – Relative Velocity Across a River

## Problem Statement

A river flows east at $v_r = 2 \text{ m/s}$. A boat, which moves at $v_b = 5 \text{ m/s}$ in still water, wants to travel directly north across the river.

Tasks:

1. Determine the angle $\theta$ relative to north at which the boat should head.
2. Calculate the time required to cross a river of width $d = 200 \text{ m}$.

## Theory

When a boat moves in a river with current, its **velocity relative to the ground** is the vector sum of:

* Velocity of the boat relative to water: $\vec{v}_b$
* Velocity of the river current: $\vec{v}_r$

To move **directly north**, the eastward component of the boat must **cancel the river current**:

$$
v_b \sin\theta = v_r
$$

where $\theta$ is the angle of the boat's heading **east of north**.

The **northward component** of the boat's velocity is:

$$
v_{\text{north}} = v_b \cos\theta
$$

Time to cross the river:

$$
t = \frac{d}{v_{\text{north}}}
$$

## Step-by-Step Solution

### Step 1: Determine heading angle

The eastward component of the boat cancels the river:

$$
v_b \sin\theta = v_r
$$

$$
\sin\theta = \frac{v_r}{v_b}
$$

$$
\sin\theta = \frac{2}{5} = 0.4
$$

$$
\theta = \arcsin(0.4)
$$

$$
\theta \approx 23.58^\circ
$$

**Conclusion:** The boat should head **$23.58^\circ$ east of north**.

### Step 2: Compute northward velocity

$$
v_{\text{north}} = v_b \cos\theta
$$

$$
v_{\text{north}} = 5 \cdot \cos(23.58^\circ)
$$

$$
v_{\text{north}} \approx 5 \cdot 0.917 = 4.585 \text{ m/s}
$$

### Step 3: Compute time to cross the river

$$
t = \frac{d}{v_{\text{north}}}
$$

$$
t = \frac{200}{4.585}
$$

$$
t \approx 43.6 \text{ s}
$$

## Final Result

* Heading angle: $\theta \approx 23.6^\circ$ east of north
* Time to cross: $t \approx 43.6 \text{ s}$

## Interpretation

By heading slightly **east of north**, the boat cancels the eastward river current and moves directly north. The crossing time is determined only by the **northward component** of the boat’s velocity.
