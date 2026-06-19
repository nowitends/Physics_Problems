## 10. Infinite Series

An ant starts at the origin and moves as follows:

- \(1\) m east
- \(1/2\) m north
- \(1/3\) m west
- \(1/4\) m south
- \(1/5\) m east
- and so on

We analyze horizontal and vertical motion separately.

---

### Step 1 — Horizontal displacement

Horizontal moves are:

\[
1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \frac{1}{9} - \cdots
\]

This is the Leibniz series:

\[
1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \cdots = \frac{\pi}{4}
\]

So the final horizontal displacement is:

\[
x = \frac{\pi}{4}
\]

---

### Step 2 — Vertical displacement

Vertical moves are:

\[
\frac{1}{2} - \frac{1}{4} + \frac{1}{6} - \frac{1}{8} + \cdots
\]

Factor out \(1/2\):

\[
\frac{1}{2}\left(1 - \frac{1}{2} + \frac{1}{3} - \frac{1}{4} + \cdots \right)
\]

We use the known series:

\[
1 - \frac{1}{2} + \frac{1}{3} - \frac{1}{4} + \cdots = \ln 2
\]

So the final vertical displacement is:

\[
y = \frac{1}{2}\ln 2
\]

---

### Final Answer

The final position of the ant is:

\[
\left(\frac{\pi}{4}, \frac{1}{2}\ln 2\right)
\]

Approximate values:

\[
x \approx 0.785, \qquad y \approx 0.347
\]
