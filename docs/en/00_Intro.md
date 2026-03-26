# Section 0: Mathematical Foundations - Solutions

## 1. Vector Algebra

**a) Magnitude of each vector**
The magnitude is calculated using $|\vec{v}| = \sqrt{x^2 + y^2 + z^2}$.
$$\vec{a} = [2, 1, -3] \implies |\vec{a}| = \sqrt{2^2 + 1^2 + (-3)^2} = \sqrt{14} \approx 3.74$$
$$\vec{b} = [4, -2, 1] \implies |\vec{b}| = \sqrt{4^2 + (-2)^2 + 1^2} = \sqrt{21} \approx 4.58$$

**b) Dot product $\vec{a} \cdot \vec{b}$**
$$\vec{a} \cdot \vec{b} = (2 \times 4) + (1 \times -2) + (-3 \times 1) = 8 - 2 - 3 = 3$$

**c) Cross product $\vec{a} \times \vec{b}$**

$$\vec{a} \times \vec{b} = \begin{vmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\ 2 & 1 & -3 \\ 4 & -2 & 1 \end{vmatrix}$$
$$= \mathbf{i}(1 - 6) - \mathbf{j}(2 - (-12)) + \mathbf{k}(-4 - 4) = [-5, -14, -8]$$

**d) Angle between vectors**
Using $\cos \theta = \frac{\vec{a} \cdot \vec{b}}{|\vec{a}||\vec{b}|}$:
$$\cos \theta = \frac{3}{\sqrt{14}\sqrt{21}} \approx 0.175 \implies \theta = \arccos(0.175) \approx 79.9^\circ$$

---

## 2. Systems of Equations
Given:
1) $2x + 3y = 12$
2) $x - y = 1 \implies x = y + 1$

Substitute (2) into (1):
$$2(y + 1) + 3y = 12 \implies 2y + 2 + 3y = 12 \implies 5y = 10 \implies y = 2$$
$$x = 2 + 1 = 3$$
**Solution: $(3, 2)$**

---

## 3. Proportionality
$$F_{new} = G \frac{(\frac{1}{2}m_1)(\frac{1}{2}m_2)}{(2r)^2} = G \frac{\frac{1}{4}m_1m_2}{4r^2} = \frac{1}{16} \left( G \frac{m_1 m_2}{r^2} \right)$$
**The force $F$ changes by a factor of $\frac{1}{16}$.**

---

## 4. Rearranging Formulas
$$T = 2\pi \sqrt{\frac{L}{g}} \implies \frac{T}{2\pi} = \sqrt{\frac{L}{g}}$$
Square both sides:
$$\frac{T^2}{4\pi^2} = \frac{L}{g} \implies g = \frac{4\pi^2 L}{T^2}$$

---

## 5. Trigonometry

$$A_x = 15 \cos(60^\circ) = 15 \times 0.5 = 7.5$$
$$A_y = 15 \sin(60^\circ) = 15 \times \frac{\sqrt{3}}{2} \approx 12.99$$

---

## 6. Function Analysis
$f(x) = 3x^2 - 12x + 7$
Find the derivative: $f'(x) = 6x - 12$. Set to zero: $6x = 12 \implies x = 2$.
Second derivative: $f''(x) = 6$. Since $f''(x) > 0$, the point is a **local minimum**.
$$f(2) = 3(2)^2 - 12(2) + 7 = 12 - 24 + 7 = -5$$
**Minimum at $(2, -5)$.**

---

## 7. Logic & Series
The time for the bicycle to reach the wall:
$$t = \frac{\text{distance}}{\text{speed}} = \frac{10\text{ m}}{1\text{ m/s}} = 10\text{ s}$$
The fly travels at $2\text{ m/s}$ for the entire $10$ seconds:
$$d = 2\text{ m/s} \times 10\text{ s} = 20\text{ m}$$

---

## 8. Definite Integrals
$$\int_{0}^{\pi} \sin(x) \, dx = [-\cos(x)]_{0}^{\pi} = -\cos(\pi) - (-\cos(0))$$
$$= -(-1) - (-1) = 1 + 1 = 2$$

---

## 9. Optimization Problem
Maximize $A = x \cdot y = x(3 - x^2) = 3x - x^3$ for $x > 0$.
$$A'(x) = 3 - 3x^2 = 0 \implies x^2 = 1 \implies x = 1$$
$$y = 3 - (1)^2 = 2$$
**Dimensions: $1 \times 2$.**

---

## 10. Infinite Series
**East/West ($x$):** $1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} \dots = \sum_{n=0}^{\infty} \frac{(-1)^n}{2n+1} = \frac{\pi}{4}$
**North/South ($y$):** $\frac{1}{2} - \frac{1}{4} + \frac{1}{6} - \frac{1}{8} \dots = \frac{1}{2} \left( 1 - \frac{1}{2} + \frac{1}{3} - \frac{1}{4} \dots \right) = \frac{\ln(2)}{2}$
**Final position:** $\left( \frac{\pi}{4}, \frac{\ln 2}{2} \right)$