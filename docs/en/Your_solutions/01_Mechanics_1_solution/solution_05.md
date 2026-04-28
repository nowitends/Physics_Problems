# Solution 5: Relative Velocity

## Problem Statement
- **River velocity ($v_r$):** 2 m/s East
- **Boat velocity in still water ($v_b$):** 5 m/s
- **Goal:** Travel directly North (perpendicular to the bank)
- **River width ($W$):** 200 meters

---

## 1. Finding the Direction (Angle)
To travel directly North, the horizontal component of the boat's velocity must exactly cancel out the river's eastward velocity.

Let $\theta$ be the angle measured from the North direction toward the West.
The boat's velocity components are:
* $v_{bx} = v_b \cdot \sin(\theta)$ (Westward)
* $v_{by} = v_b \cdot \cos(\theta)$ (Northward)

**Condition for straight North travel:**
$$v_b \cdot \sin(\theta) = v_r$$
$$5 \cdot \sin(\theta) = 2$$
$$\sin(\theta) = \frac{2}{5} = 0.4$$
$$\theta = \arcsin(0.4) \approx \mathbf{23.58^\circ}$$

**Result:** The boat should head at an angle of approximately **$23.58^\circ$ West of North**.

---

## 2. Calculating the Time to Cross
The time taken to cross the river depends only on the northward (vertical) component of the velocity ($v_{by}$).

**First, find $v_{by}$:**
$$v_{by} = v_b \cdot \cos(\theta)$$
Since $\sin(\theta) = 0.4$, we use $\cos(\theta) = \sqrt{1 - \sin^2(\theta)} = \sqrt{1 - 0.16} = \sqrt{0.84} \approx 4.58 \text{ m/s}$.

**Calculate Time ($t$):**
$$t = \frac{\text{Width}}{v_{by}}$$
$$t = \frac{200 \text{ m}}{4.58 \text{ m/s}} \approx \mathbf{43.67 \text{ seconds}}$$

**Result:** It will take approximately **43.67 seconds** to cross the river.
