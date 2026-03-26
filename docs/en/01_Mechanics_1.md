# Section 1: Mechanics I - Solutions

## 1. Projectile Motion
Given: $v_0 = 100 \text{ m/s}$, $\theta = 37^\circ$, $g \approx 9.8 \text{ m/s}^2$.
Horizontal component: $v_{0x} = 100 \cos(37^\circ) \approx 80 \text{ m/s}$.
Vertical component: $v_{0y} = 100 \sin(37^\circ) \approx 60 \text{ m/s}$.



* **Differential Equations:**
  $$\frac{d^2x}{dt^2} = 0, \quad \frac{d^2y}{dt^2} = -g$$
* **Time of Flight ($T$):**
  $$y(T) = v_{0y}T - \frac{1}{2}gT^2 = 0 \implies T = \frac{2v_{0y}}{g} = \frac{120}{9.8} \approx 12.24 \text{ s}$$
* **Maximum Height ($H$):**
  $$H = \frac{v_{0y}^2}{2g} = \frac{60^2}{2(9.8)} \approx 183.67 \text{ m}$$
* **Range ($R$):**
  $$R = v_{0x}T = 80 \times 12.24 \approx 979.2 \text{ m}$$

---

## 2. Range Optimization
The range formula is $R(\theta) = \frac{v_0^2 \sin(2\theta)}{g}$. To find the maximum:
$$\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot 2\cos(2\theta) = 0$$
$$\cos(2\theta) = 0 \implies 2\theta = 90^\circ \implies \theta = 45^\circ$$
Since $\frac{d^2R}{d\theta^2} < 0$ at $45^\circ$, the range is maximized at **45 degrees**.

---

## 3. Path Intersection
Alice: $\vec{A}(t) = (2+t, 8-3t)$. Bob: $\vec{B}(t) = (2t-1, 2t+2)$.
Set $x_A = x_B$:
$$2+t = 2t-1 \implies t = 3$$
Check $y$ values at $t=3$:
$$y_A(3) = 8 - 3(3) = -1$$
$$y_B(3) = 2(3) + 2 = 8$$
Since $y_A \neq y_B$ at the same time, they **do not collide**.
To find the **minimum distance**, minimize $f(t) = |\vec{A}(t) - \vec{B}(t)|^2$:
$$D^2 = (3-t)^2 + (6-5t)^2 = 26t^2 - 66t + 45$$
$$f'(t) = 52t - 66 = 0 \implies t \approx 1.27 \text{ s}$$
$$D_{min} \approx \sqrt{26(1.27)^2 - 66(1.27) + 45} \approx 1.76 \text{ m}$$

---

## 4. Vector Calculus
Position: $\vec{r}(t) = (3t^2)\hat{i} + (5t - 8t^2)\hat{j}$
* **Velocity:** $\vec{v}(t) = \frac{d\vec{r}}{dt} = (6t)\hat{i} + (5 - 16t)\hat{j}$
* **Acceleration:** $\vec{a}(t) = \frac{d\vec{v}}{dt} = 6\hat{i} - 16\hat{j}$

---

## 5. Relative Velocity
River flow: $\vec{v}_r = 2 \text{ m/s}$ (East). Boat speed: $v_b = 5 \text{ m/s}$.
To go North, the boat must counteract the Eastward flow:
$$\sin \theta = \frac{v_{river}}{v_{boat}} = \frac{2}{5} = 0.4 \implies \theta \approx 23.58^\circ \text{ West of North}$$
Northward speed: $v_N = 5 \cos(23.58^\circ) \approx 4.58 \text{ m/s}$.
Time: $t = \frac{200 \text{ m}}{4.58 \text{ m/s}} \approx 43.67 \text{ s}$.

---

## 6. Variable Velocity
$v(t) = t^2 + 2t - 5$, $x(0) = 4$.
* **Acceleration:** $a(t) = v'(t) = 2t + 2 \implies a(3) = 8 \text{ m/s}^2$.
* **Position:** $x(t) = \int v(t) dt = \frac{1}{3}t^3 + t^2 - 5t + C$.
Using $x(0)=4 \implies C=4$.
$$x(3) = \frac{1}{3}(27) + 9 - 15 + 4 = 7 \text{ m}$$

---

## 7. Elimination of Time
$x = 2t^2 \implies t = \sqrt{x/2}$.
* **Trajectory:** $y = 3(x/2)^{3/2} = \frac{3}{2\sqrt{2}}x^{3/2}$.
* **Vectors:**
$$\vec{v}(t) = [4t, 9t^2], \quad |\vec{v}(t)| = \sqrt{16t^2 + 81t^4}$$
$$\vec{a}(t) = [4, 18t], \quad |\vec{a}(t)| = \sqrt{16 + 324t^2}$$
The acceleration is **not constant** because it depends on $t$.

---

## 8. Circular Motion
$R = 6.378 \times 10^6 \text{ m}$, $T = 86400 \text{ s}$.
$$a_c = \omega^2 R = \left(\frac{2\pi}{T}\right)^2 R$$
$$a_c = (7.27 \times 10^{-5})^2 \times 6.378 \times 10^6 \approx 0.0337 \text{ m/s}^2$$

---

## 9. Momentum Comparison
$p = mv$
* Fly: $p = 0.002 \text{ kg} \times 10 \text{ m/s} = 0.02 \text{ kg}\cdot\text{m/s}$
* Ball: $p = 0.06 \text{ kg} \times 1 \text{ m/s} = 0.06 \text{ kg}\cdot\text{m/s}$
The **tennis ball** has greater momentum.

---

## 10. Kinematics (3D)
$\vec{r}(t) = (a \cos(\omega t), b \sin(\omega t), bt)$



**a) Trajectory:**
The $xy$ projections follow $\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1$. Combined with $z=bt$, the path is an **elliptical helix**.

**b) Path Length ($s$):**
$$\vec{v}(t) = (-a\omega \sin \omega t, b\omega \cos \omega t, b)$$
$$s = \int_0^{t_0} \sqrt{a^2\omega^2 \sin^2(\omega t) + b^2\omega^2 \cos^2(\omega t) + b^2} \, dt$$