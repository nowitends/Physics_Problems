## 8. Waves - Wave Equation Verification

**Problem:**
Which of the following functions can describe a traveling wave? Hint: Check if it satisfies the wave equation:
$$\frac{\partial^2 y}{\partial x^2} = \frac{1}{v^2} \frac{\partial^2 y}{\partial t^2}$$

a) $y(x, t) = A \cos(kx^2 - \omega t)$
b) $y(x, t) = A(x - vt)^2$
c) $y(x, t) = A \log(x + vt)$

**Solution:**
A function $y(x, t)$ describes a traveling wave if it is in the form $f(x - vt)$ (moving in the $+x$ direction) or $f(x + vt)$ (moving in the $-x$ direction). Alternatively, it must satisfy the linear second-order wave equation.

### 8.a) $y(x, t) = A \cos(kx^2 - \omega t)$
* **Analysis:** The argument $(kx^2 - \omega t)$ is not a linear function of $x$ and $t$. In a true traveling wave, $x$ and $t$ must appear as a linear combination $(ax \pm bt)$.
* **Result:** **No**, this does not describe a standard traveling wave.

### 8.b) $y(x, t) = A(x - vt)^2$
* **Analysis:** This function is in the form $f(u)$ where $u = x - vt$. Let's check the derivatives:
    * $\frac{\partial y}{\partial x} = 2A(x-vt)$ and $\frac{\partial^2 y}{\partial x^2} = 2A$
    * $\frac{\partial y}{\partial t} = -2Av(x-vt)$ and $\frac{\partial^2 y}{\partial t^2} = 2Av^2$
* **Verification:** $\frac{\partial^2 y}{\partial x^2} = 2A$ and $\frac{1}{v^2}(2Av^2) = 2A$. The equation holds.
* **Result:** **Yes**, this describes a traveling wave.

### 8.c) $y(x, t) = A \log(x + vt)$
* **Analysis:** This function is in the form $f(u)$ where $u = x + vt$. Any twice-differentiable function of the form $f(x \pm vt)$ satisfies the wave equation.
* **Result:** **Yes**, this describes a traveling wave.

**Final Answer:** Functions **(b)** and **(c)** can describe traveling waves.
