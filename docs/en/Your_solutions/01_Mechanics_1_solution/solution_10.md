Given:

r(t) = (a cos(ωt), b sin(ωt), bt)

where a, b, ω are positive constants.

---

### a) Trajectory

Coordinates are:

x = a cos(ωt)  
y = b sin(ωt)  
z = bt

From x and y:

x/a = cos(ωt)  
y/b = sin(ωt)

Using:

cos²(ωt) + sin²(ωt) = 1

we get:

(x² / a²) + (y² / b²) = 1

So in the xy-plane the trajectory is an ellipse.

Since z = bt, the point also moves upward linearly.

So the full motion is an **elliptic helix**.

---

### b) Path length from t = 0 to t = t₀

Velocity is derivative of position:

r'(t) = (-aω sin(ωt), bω cos(ωt), b)

Speed:

|r'(t)| = √(a²ω² sin²(ωt) + b²ω² cos²(ωt) + b²)

So the arc length is:

L = ∫ from 0 to t₀ √(a²ω² sin²(ωt) + b²ω² cos²(ωt) + b²) dt

This is the required path length formula.

---

### c) Special cases

- If a = b, then the ellipse becomes a circle, so the path is a circular helix.
- If b = 0 in the third coordinate term, then there is no vertical motion and the path stays in one plane.
- If ω is larger, the point rotates faster around the axis.

---

Final answer:

Trajectory in xy-plane:

(x² / a²) + (y² / b²) = 1

Full trajectory: elliptic helix

Path length:

L = ∫₀ᵗ⁰ √(a²ω² sin²(ωt) + b²ω² cos²(ωt) + b²) dt
