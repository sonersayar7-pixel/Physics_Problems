## 1. Coulomb's Law

**Problem:** Four point charges of $+1.0\text{ C}$ each are placed at the corners of a square with sides of $1.0\text{ m}$. Calculate the magnitude and direction of the electric force on a charge of $-2.0\text{ C}$ placed at the center of the square.

**Solution:**
By symmetry, the forces exerted by the charges at opposite corners are equal in magnitude but opposite in direction.
* The charge at the top-left pulls the center charge toward it.
* The charge at the bottom-right pulls the center charge toward it with the exact same magnitude.
* These two vectors cancel each other out.

The same applies to the charges on the other diagonal. Therefore, the net force is zero.
$$F_{\text{net}} = 0\text{ N}$$

---

## 2. Electric Potential

**Problem:** Point charges of $+1\text{ C}$, $-2\text{ C}$, $+3\text{ C}$, and $-4\text{ C}$ are placed at the corners of a square with sides of $1.0\text{ m}$ (in order). Calculate the electric potential at the center of the square.

**Solution:**
Electric potential $V$ is a scalar quantity. The total potential at the center is the algebraic sum of the potentials from each charge. The distance $r$ from any corner to the center of a square with side $a = 1.0\text{ m}$ is half the diagonal:
$$r = \frac{a\sqrt{2}}{2} = \frac{1.0\text{ m} \cdot \sqrt{2}}{2} = \frac{\sqrt{2}}{2}\text{ m}$$

The total potential is:
$$V_{\text{total}} = \sum \frac{k q_i}{r} = \frac{k}{r} (q_1 + q_2 + q_3 + q_4)$$
$$V_{\text{total}} = \frac{8.99 \times 10^9}{\frac{\sqrt{2}}{2}} (1 - 2 + 3 - 4)$$
$$V_{\text{total}} = \frac{8.99 \times 10^9}{0.707} (-2) \approx -2.54 \times 10^{10}\text{ V}$$

---

## 3. Electrostatic Equilibrium

**Problem:** Find the equilibrium position for a charge $q_3 = +1\text{ C}$ placed on the line between a charge $q_1 = +4\text{ C}$ and a charge $q_2 = +9\text{C}$, which are separated by a distance of $2\text{ m}$.

**Solution:**
For $q_3$ to be in equilibrium, the net electrostatic force on it must be zero. The repulsion from $q_1$ must equal the repulsion from $q_2$. Let $x$ be the distance from $q_1$. The distance from $q_2$ will be $(2 - x)$.
$$F_{13} = F_{23}$$
$$k \frac{q_1 q_3}{x^2} = k \frac{q_2 q_3}{(2-x)^2}$$

Cancel out $k$ and $q_3$:
$$\frac{4}{x^2} = \frac{9}{(2-x)^2}$$

Take the square root of both sides:
$$\frac{2}{x} = \frac{3}{2-x}$$
$$2(2 - x) = 3x$$
$$4 - 2x = 3x \implies 5x = 4$$
$$x = 0.8\text{ m}$$

The equilibrium position is **$0.8\text{ m}$ away from the $+4\text{ C}$ charge**.

---

## 4. Force Comparison

**Problem:** Calculate the magnitude of the electric force and gravitational force between an electron and a proton in a hydrogen atom ($r \approx 5.3 \times 10^{-11}\text{ m}$). What is the ratio $F_e/F_g$?

**Solution:**
**Electric Force ($F_e$):**
$$F_e = k \frac{|q_1 q_2|}{r^2} = (8.99 \times 10^9) \frac{(1.6 \times 10^{-19})^2}{(5.3 \times 10^{-11})^2}$$
$$F_e \approx 8.2 \times 10^{-8}\text{ N}$$

**Gravitational Force ($F_g$):**
$$F_g = G \frac{m_e m_p}{r^2} = (6.674 \times 10^{-11}) \frac{(9.11 \times 10^{-31})(1.67 \times 10^{-27})}{(5.3 \times 10^{-11})^2}$$
$$F_g \approx 3.6 \times 10^{-47}\text{ N}$$

**Ratio:**
$$\frac{F_e}{F_g} = \frac{8.2 \times 10^{-8}}{3.6 \times 10^{-47}} \approx 2.3 \times 10^{39}$$
The electric force is astronomically larger than the gravitational force.

---

## 5. Field Levitation

**Problem:** What electric field strength is required to make a proton levitate against Earth's gravity at the surface? 

**Solution:**
For the proton to levitate, the upward electric force must exactly balance the downward gravitational force.
$$F_e = F_g$$
$$qE = mg$$
$$E = \frac{mg}{q}$$
$$E = \frac{(1.67 \times 10^{-27}\text{ kg})(9.8\text{ m/s}^2)}{1.6 \times 10^{-19}\text{ C}}$$
$$E \approx 1.02 \times 10^{-7}\text{ V/m}$$
The electric field must point **upward** (since the proton is positively charged).

---

## 6. Field at a point from a system of charges

**Problem:** Charges $+q$ at $(-a, 0)$ and $+2q$ at $(a, 0)$.

**Solution:**

**1. General Electric Field Vectors:**
By superposition, $\vec{E} = \vec{E}_1 + \vec{E}_2$. Let $\vec{r}_1 = (x+a)\hat{i} + y\hat{j}$ and $\vec{r}_2 = (x-a)\hat{i} + y\hat{j}$.
$$\vec{E}(x,y) = k q \left[ \frac{(x+a)\hat{i} + y\hat{j}}{((x+a)^2 + y^2)^{3/2}} \right] + 2k q \left[ \frac{(x-a)\hat{i} + y\hat{j}}{((x-a)^2 + y^2)^{3/2}} \right]$$

For a point on the y-axis ($x=0$):
$$\vec{E}(0,y) = \frac{k q}{(a^2+y^2)^{3/2}} (a\hat{i} + y\hat{j}) + \frac{2k q}{(a^2+y^2)^{3/2}} (-a\hat{i} + y\hat{j})$$
$$\vec{E}(0,y) = \frac{k q}{(a^2+y^2)^{3/2}} (-a\hat{i} + 3y\hat{j})$$

For a point on the x-axis ($y=0$):
$$\vec{E}(x,0) = k q \left[ \frac{\text{sgn}(x+a)}{(x+a)^2} \hat{i} + \frac{2\text{sgn}(x-a)}{(x-a)^2} \hat{i} \right]$$

**2. Condition for Zero Components:**
* $E_y = 0$: Only occurs when $y = 0$.
* $E_x = 0$ (and $\vec{E} = 0$): This must occur on the x-axis between the charges ($-a < x < a$), where vectors oppose each other.
    $$\frac{k q}{(x+a)^2} = \frac{2k q}{(a-x)^2}$$
    $$(a-x)^2 = 2(x+a)^2 \implies x = a(-3 + 2\sqrt{2}) \approx -0.17a$$

**3. Specific Calculation ($a=0.2$, $y=0.3$, $q=2\mu\text{C}$):**
Using the $\vec{E}(0,y)$ equation:
$$\vec{E}(0, 0.3) = \frac{(8.99 \times 10^9)(2 \times 10^{-6})}{(0.2^2 + 0.3^2)^{3/2}} (-0.2\hat{i} + 3(0.3)\hat{j})$$
$$\vec{E}(0, 0.3) \approx 3.84 \times 10^5 (-0.2\hat{i} + 0.9\hat{j})\text{ V/m}$$
$$\vec{E} = (-7.68 \times 10^4 \hat{i} + 3.46 \times 10^5 \hat{j})\text{ V/m}$$

**4. Limit $y \gg a$:**
If $y \gg a$, then $(a^2 + y^2) \approx y^2$. The $\hat{i}$ components from the $-a$ shift become negligible compared to the massive vertical distance.
$$\vec{E}(0, y) \approx \frac{kq}{(y^2)^{3/2}}(3y\hat{j}) = \frac{3kq}{y^2}\hat{j}$$
This makes sense, as viewed from far away, the system acts like a single point charge of $+3q$ at the origin.

---

## 7. Cyclotron Motion

**Problem:** An electron is accelerated through $5000\text{ V}$, then enters a uniform magnetic field $B = 0.1\text{ T}$ perpendicular to its velocity. What is the radius of the path?

**Solution:**
First, find the velocity from kinetic energy:
$$\frac{1}{2} m v^2 = e V \implies v = \sqrt{\frac{2 e V}{m}}$$
$$v = \sqrt{\frac{2(1.6 \times 10^{-19})(5000)}{9.11 \times 10^{-31}}} \approx 4.19 \times 10^7\text{ m/s}$$

Equate centripetal force with the magnetic Lorentz force to find radius $r$:
$$F_B = F_c \implies e v B = \frac{m v^2}{r} \implies r = \frac{m v}{e B}$$
$$r = \frac{(9.11 \times 10^{-31})(4.19 \times 10^7)}{(1.6 \times 10^{-19})(0.1)}$$
$$r \approx 2.38 \times 10^{-3}\text{ m} \quad (\text{or } 2.38\text{ mm})$$

---

## 8. Lorentz Force

**Problem:** $q = 2 \times 10^{-19}\text{ C}$, $m = 4 \times 10^{-27}\text{ kg}$, enters $B = 0.5\text{ T}$ at $v = 10^6\text{ m/s}$ perpendicularly. Magnitude of the Lorentz force?

**Solution:**
Since the velocity is perpendicular to the magnetic field ($\theta = 90^\circ$):
$$F = q v B \sin(90^\circ) = q v B$$
$$F = (2 \times 10^{-19}\text{ C}) \cdot (10^6\text{ m/s}) \cdot (0.5\text{ T})$$
$$F = 1.0 \times 10^{-13}\text{ N}$$

---

## 9. Vector Lorentz Force

**Problem:** A proton moves with $\vec{v} = (2\hat{i} - 4\hat{j} + \hat{k})\text{ m/s}$ in $\vec{B} = (\hat{i} + 2\hat{j} - \hat{k})\text{ T}$. Magnitude of magnetic force?

**Solution:**
The magnetic force is given by the cross product $\vec{F} = q(\vec{v} \times \vec{B})$.
$$\vec{v} \times \vec{B} = \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ 2 & -4 & 1 \\ 1 & 2 & -1 \end{vmatrix}$$
$$\vec{v} \times \vec{B} = \hat{i}((-4)(-1) - (1)(2)) - \hat{j}((2)(-1) - (1)(1)) + \hat{k}((2)(2) - (-4)(1))$$
$$\vec{v} \times \vec{B} = \hat{i}(4 - 2) - \hat{j}(-2 - 1) + \hat{k}(4 + 4) = 2\hat{i} + 3\hat{j} + 8\hat{k}$$

Find the magnitude of the cross product:
$$|\vec{v} \times \vec{B}| = \sqrt{2^2 + 3^2 + 8^2} = \sqrt{4 + 9 + 64} = \sqrt{77} \approx 8.775$$

Now multiply by the charge of a proton ($q = 1.6 \times 10^{-19}\text{ C}$):
$$F = q|\vec{v} \times \vec{B}| = (1.6 \times 10^{-19}) \cdot \sqrt{77}$$
$$F \approx 1.4 \times 10^{-18}\text{ N}$$

---

## 10. Lorentz Force acting on Wire

**Problem:** A $2.0\text{ m}$ wire carries $10\text{ A}$ in a $B = 0.5\text{ T}$ field. Calculate the force for angles of $90^\circ$, $45^\circ$, and $0^\circ$.

**Solution:**
The magnetic force on a current-carrying wire is $F = I L B \sin\theta$.
Max Force $F_{\text{max}} = (10\text{ A})(2.0\text{ m})(0.5\text{ T}) = 10\text{ N}$.

* **a) $90^\circ$**
    $$F = 10 \sin(90^\circ) = 10\text{ N}$$
* **b) $45^\circ$**
    $$F = 10 \sin(45^\circ) = 10 \left(\frac{\sqrt{2}}{2}\right) = 5\sqrt{2} \approx 7.07\text{ N}$$
* **c) $0^\circ$**
    $$F = 10 \sin(0^\circ) = 0\text{ N}$$