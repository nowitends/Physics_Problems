#  Electromagnetic Wave Analysis 

## 🧾 Given

Electric field:

$$
E_y(x,t) = 100 \sin(10^7 x - \omega t) , \text{V/m}
$$

---

## 🎯 Objectives

Find:

1. Direction of propagation
2. Wavelength (\lambda)
3. Angular frequency (\omega)
4. Magnetic field equation

---

## 📐 Step 1: Identify Wave Form

The general form of a traveling wave is:

$$
E(x,t) = E_0 \sin(kx - \omega t)
$$

### Explanation:

* (k) → wave number
* (\omega) → angular frequency
* The sign determines direction of propagation

---

## 📌 Step 2: Direction of Propagation

Given expression:

$$
\sin(10^7 x - \omega t)
$$

### Explanation:

* A wave of the form (\sin(kx - \omega t)) travels in the **+x direction**
* A wave of the form (\sin(kx + \omega t)) travels in the **–x direction**

👉 Therefore:

$$
\text{Direction} = +x
$$

---

## 📌 Step 3: Identify Wave Number (k)

From the equation:

$$
k = 10^7 , \text{rad/m}
$$

---

## 📌 Step 4: Calculate Wavelength

Using:

$$
\lambda = \frac{2\pi}{k}
$$

---

### Calculation:

$$
\lambda = \frac{2\pi}{10^7}
$$

$$
\lambda \approx 6.28 \times 10^{-7} , m
$$

---

## 📌 Step 5: Calculate Angular Frequency

For electromagnetic waves:

$$
c = \frac{\omega}{k}
$$

Where:

* (c = 3 \times 10^8 , m/s)

---

### Solve for (\omega):

$$
\omega = c \cdot k
$$

$$
\omega = (3 \times 10^8)(10^7)
$$

$$
\omega = 3 \times 10^{15} , \text{rad/s}
$$

---

## 📌 Step 6: Magnetic Field Equation

Using relation from Electromagnetic Wave:

$$
B_0 = \frac{E_0}{c}
$$

---

### Calculate Magnetic Field Amplitude:

$$
B_0 = \frac{100}{3 \times 10^8}
$$

$$
B_0 \approx 3.33 \times 10^{-7} , T
$$

---

### Write Full Magnetic Field:

$$
B_z(x,t) = B_0 \sin(10^7 x - \omega t)
$$

$$
B_z(x,t) = 3.33 \times 10^{-7} \sin(10^7 x - \omega t)
$$

---

### Explanation:

* Electric field is in **y-direction**
* Wave travels in **x-direction**
* Therefore magnetic field must be in **z-direction** (right-hand rule)

---

## ✅ Final Results

* Direction of propagation:

$$

* x \text{ direction}
  $$

- Wavelength:

$$
\lambda \approx 6.28 \times 10^{-7} , m
$$

* Angular frequency:

$$
\omega = 3 \times 10^{15} , \text{rad/s}
$$

* Magnetic field:

$$
B_z(x,t) = 3.33 \times 10^{-7} \sin(10^7 x - \omega t)
$$

---
