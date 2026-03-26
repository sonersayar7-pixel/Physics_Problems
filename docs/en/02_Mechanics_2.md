# Section 2: Mechanics II - Solutions

## 1. Gravitational Dependence
The period of a simple pendulum is $T = 2\pi\sqrt{L/g}$.
* **On the Moon:** Since $g_{moon} = g_{earth}/6$, then $T \propto 1/\sqrt{g}$.
  $$T_{moon} = T_{earth} \times \sqrt{6} = 4 \times 2.45 \approx 9.80 \text{ s}$$
* **Length for 1s period on Earth:**
  $$1 = 2\pi\sqrt{\frac{L}{9.8}} \implies L = \frac{9.8}{4\pi^2} \approx 0.248 \text{ m (24.8 cm)}$$

---

## 2. Harmonic Motion
$x(t) = 0.2 \cos(10\pi t)$. General form: $x(t) = A \cos(\omega t)$.
* **Spring Constant ($k$):** $\omega = 10\pi$. Since $\omega = \sqrt{k/m}$:
  $$k = m\omega^2 = 10 \times (10\pi)^2 = 1000\pi^2 \approx 9870 \text{ N/m}$$
* **Total Energy ($E$):**
  $$E = \frac{1}{2}kA^2 = \frac{1}{2}(1000\pi^2)(0.2)^2 = 20\pi^2 \approx 197.4 \text{ J}$$

---

## 3. Conservation of Energy
Using $mgh = \frac{1}{2}mv^2$. The height $h = L(1 - \cos\theta)$.

$$h = 1.0(1 - \cos 15^\circ) \approx 1.0(1 - 0.966) = 0.034 \text{ m}$$
$$v = \sqrt{2gh} = \sqrt{2 \times 9.8 \times 0.034} \approx 0.816 \text{ m/s}$$

---

## 4. Energy & Momentum
1. **Speed at bottom ($v_1$):** $mgh = \frac{1}{2}mv_1^2 \implies v_1 = \sqrt{2(9.8)(3.0)} = 7.67 \text{ m/s}$.
2. **Inelastic Collision:** $m_1v_1 = (m_1 + m_2)v_f$.
   $$0.5 \times 7.67 = (0.5 + 1.5)v_f \implies 3.835 = 2v_f \implies v_f \approx 1.92 \text{ m/s}$$

---

## 5. Inelastic Collision
Conservation of momentum: $m_r v_r = (m_r + m_c)v_f$.
$$70 \times 3 = (70 + 140)v_f \implies 210 = 210v_f \implies v_f = 1 \text{ m/s}$$
**Is energy conserved?** No. 
Initial $KE = \frac{1}{2}(70)(3^2) = 315 \text{ J}$. 
Final $KE = \frac{1}{2}(210)(1^2) = 105 \text{ J}$. 
Energy is lost to heat/deformation.

---

## 6. Energy Dissipation
Initial energy $E_0 = mgh_0$. After 1 bounce: $E_1 = 0.7 E_0$. After 2 bounces: $E_2 = (0.7)^2 E_0 = 0.49 E_0$.
Since $E \propto h$:
$$h_2 = 0.49 \times 2.0 = 0.98 \text{ m}$$

---

## 7. Dynamics with Friction
Forces on the 10kg block ($M$): Applied force $F=45$N, friction from ground $f_1$, friction from top block $f_2$.
$\mu = 0.2, m = 5\text{kg}, M = 10\text{kg}$.
* $f_2 = \mu mg = 0.2(5)(9.8) = 9.8$ N (Top block is tied, so it resists $M$'s motion).
* $f_1 = \mu(m+M)g = 0.2(15)(9.8) = 29.4$ N.
$$\sum F = F - f_1 - f_2 = 45 - 29.4 - 9.8 = 5.8 \text{ N}$$
$$a = \frac{5.8}{10} = 0.58 \text{ m/s}^2$$

---

## 8. Work of a Variable Force
* **Equation of Motion:** $m\frac{d^2x}{dt^2} = -kx$. Solution: $x(t) = A\cos(\omega t + \phi)$ where $\omega = \sqrt{k/m}$.
* **Work:** $W = \int_0^{x_0} F(x) dx = \int_0^{x_0} -kx dx = [-\frac{1}{2}kx^2]_0^{x_0} = -\frac{1}{2}kx_0^2$.
* **Potential Energy:** $U(x) = -W = \frac{1}{2}kx^2$.
* **Verification:** $-\frac{dU}{dx} = -\frac{d}{dx}(\frac{1}{2}kx^2) = -kx = F$.

---

## 9. Vertical Throw with Drag
$m\frac{dv}{dt} = -mg - kv \implies \frac{dv}{dt} = -(g + \frac{k}{m}v)$.
Separating variables and integrating:
$$v(t) = (v_0 + \frac{mg}{k})e^{-\frac{k}{m}t} - \frac{mg}{k}$$

**Max Height:** Occurs when $v(t)=0$. Compared to the vacuum case ($h = v_0^2/2g$), the drag case reaches a lower height because energy is dissipated.

---

## 10. Force Field and Power
$m = 0.5$ kg.
* **Velocity ($\vec{v}$):** $\frac{d}{dt}(5t^2-t, 2t^3, -3t+2) = (10t-1, 6t^2, -3) \text{ m/s}$.
* **Momentum ($\vec{p}$):** $m\vec{v} = (5t-0.5, 3t^2, -1.5) \text{ kg}\cdot\text{m/s}$.
* **Acceleration ($\vec{a}$):** $\frac{d\vec{v}}{dt} = (10, 12t, 0) \text{ m/s}^2$.
* **Force ($\vec{F}$):** $m\vec{a} = (5, 6t, 0) \text{ N}$.
* **Power ($P$):** $\vec{F} \cdot \vec{v} = 5(10t-1) + 6t(6t^2) + 0 = 36t^3 + 50t - 5 \text{ W}$.

---

## 11. Dynamics with a Time-Dependent Force
$\vec{a} = \frac{\vec{F}}{m} = (5t, t-4, -2t^2)$.
* **Velocity:** $\vec{v}(t) = \int \vec{a} dt + \vec{v}_0 = (\frac{5}{2}t^2+2, \frac{1}{2}t^2-4t, -\frac{2}{3}t^3+1)$.
* **Position:** $\vec{r}(t) = \int \vec{v} dt + \vec{r}_0 = (\frac{5}{6}t^3+2t+5, \frac{1}{6}t^3-2t^2+2, -\frac{1}{6}t^4+t-3)$.

---

## 12. Work and Energy with a Constant Force
$\vec{F} = [6, 2], m = 2$.
* **$\vec{a}(t)$:** $\vec{F}/m = [3, 1] \text{ m/s}^2$.
* **$\vec{v}(t)$:** $\vec{v}_0 + \vec{a}t = (3t+1, t-1) \text{ m/s}$.
* **$\vec{r}(t)$:** $\vec{r}_0 + \vec{v}_0t + \frac{1}{2}\vec{a}t^2 = (\frac{3}{2}t^2+t, \frac{1}{2}t^2-t) \text{ m}$.
* **Work ($W$) at $t=3$:** $\Delta\vec{r}(3) = (16.5, 1.5)$.
  $$W = \vec{F} \cdot \Delta\vec{r} = 6(16.5) + 2(1.5) = 99 + 3 = 102 \text{ J}$$
* **Work-Energy Theorem:** $\Delta KE = \frac{1}{2}m(v_f^2 - v_i^2)$.
  $v_i^2 = 1^2 + (-1)^2 = 2$. At $t=3, \vec{v}(3) = (10, 2) \implies v_f^2 = 104$.
  $\Delta KE = \frac{1}{2}(2)(104 - 2) = 102 \text{ J}$. (Consistent).