## 1. Coulomb's Law

**Problem:** Four point charges of $+1.0\text{ C}$ each are placed at the corners of a square with sides of $1.0\text{ m}$. Calculate the magnitude and direction of the electric force on a charge of $-2.0\text{ C}$ placed at the center of the square.

**Solution:**
To find the net force on the central charge, we must use the principle of superposition, which states that the total force is the vector sum of the individual forces exerted by each corner charge. 

Let's analyze the symmetry of the system:
1. The distance $r$ from any corner to the center of the square is identical for all four charges.
2. The magnitude of the force exerted by any single $+1.0\text{ C}$ charge on the central $-2.0\text{ C}$ charge is given by Coulomb's Law: $F = k \frac{|q_1 q_2|}{r^2}$. Because the charges and distances are identical, the magnitude of the pull from each corner is exactly the same.
3. Because the center charge is negative and the corner charges are positive, the forces are strictly attractive. The central charge is pulled directly toward each corner.

Now, consider the charges at opposite diagonal corners (e.g., top-left and bottom-right). The top-left charge pulls the central charge up and to the left. The bottom-right charge pulls the central charge down and to the right with the exact same magnitude of force. These two force vectors are $180^\circ$ apart and perfectly cancel each other out. 

The exact same cancellation happens with the top-right and bottom-left charges. Since all individual force vectors perfectly oppose each other in pairs, the net electrostatic force is zero.

$$F_{\text{net}} = 0\text{ N}$$

---

## 2. Electric Potential

**Problem:** Point charges of $+1\text{ C}$, $-2\text{ C}$, $+3\text{ C}$, and $-4\text{ C}$ are placed at the corners of a square with sides of $1.0\text{ m}$ (in order). Calculate the electric potential at the center of the square.

**Solution:**
Unlike electric force, which is a vector, electric potential ($V$) is a scalar quantity. This makes our calculation much simpler, as we do not need to worry about vector angles or cancellations. We simply calculate the potential created by each charge at the center and add them together algebraically (keeping their positive or negative signs).

First, we need to find the distance $r$ from the corners to the center. For a square with side length $a = 1.0\text{ m}$, the length of the full diagonal is given by the Pythagorean theorem as $a\sqrt{2}$. The center is exactly halfway along the diagonal:
$$r = \frac{a\sqrt{2}}{2} = \frac{1.0\text{ m} \cdot \sqrt{2}}{2} \approx 0.707\text{ m}$$

The principle of superposition for electric potential states:
$$V_{\text{total}} = V_1 + V_2 + V_3 + V_4 = \sum \frac{k q_i}{r}$$

Since $k$ (Coulomb's constant, $\approx 8.99 \times 10^9\text{ N}\cdot\text{m}^2/\text{C}^2$) and $r$ are common to all terms, we can factor them out:
$$V_{\text{total}} = \frac{k}{r} (q_1 + q_2 + q_3 + q_4)$$

Plug in the values, being careful to include the negative signs of the charges:
$$V_{\text{total}} = \frac{8.99 \times 10^9}{0.707} (+1 - 2 + 3 - 4)$$
$$V_{\text{total}} = (1.27 \times 10^{10}) \cdot (-2)$$
$$V_{\text{total}} \approx -2.54 \times 10^{10}\text{ V}$$

The total electric potential at the center of the square is approximately $-2.54 \times 10^{10}\text{ Volts}$.

---

## 3. Electrostatic Equilibrium

**Problem:** Find the equilibrium position for a charge $q_3 = +1\text{ C}$ placed on the line between a charge $q_1 = +4\text{ C}$ and a charge $q_2 = +9\text{C}$, which are separated by a distance of $2\text{ m}$.

**Solution:**
For a particle to be in "electrostatic equilibrium," the net electrostatic force acting on it must be zero. 
Because $q_1$ and $q_2$ are both positive, they will both repel the positive test charge $q_3$. 
* If we place $q_3$ to the left of $q_1$ or the right of $q_2$, both forces would push it in the same direction, so equilibrium is impossible there. 
* Therefore, the equilibrium point must lie *between* the two charges, where the repulsion from $q_1$ pushes right and the repulsion from $q_2$ pushes left.

Let $x$ be the distance from $q_1$ to the equilibrium point. Because the total distance is $2\text{ m}$, the distance from $q_2$ to the equilibrium point will be $(2 - x)$.

For equilibrium, the magnitudes of the two opposing forces must be equal:
$$F_{13} = F_{23}$$
$$k \frac{|q_1 q_3|}{x^2} = k \frac{|q_2 q_3|}{(2-x)^2}$$

Notice that Coulomb's constant $k$ and the magnitude of the test charge $q_3$ appear on both sides. We can divide both sides by $k \cdot q_3$ to simplify the equation immensely:
$$\frac{q_1}{x^2} = \frac{q_2}{(2-x)^2}$$
$$\frac{4}{x^2} = \frac{9}{(2-x)^2}$$

To avoid solving a quadratic equation, we can take the square root of both sides (since physical distances are positive here, we only care about the positive roots):
$$\frac{2}{x} = \frac{3}{2-x}$$

Now, cross-multiply to solve for $x$:
$$2(2 - x) = 3x$$
$$4 - 2x = 3x$$
$$4 = 5x \implies x = \frac{4}{5} = 0.8\text{ m}$$

The equilibrium position is located **$0.8\text{ m}$ away from the $+4\text{ C}$ charge** (and $1.2\text{ m}$ away from the $+9\text{ C}$ charge).

---

## 4. Force Comparison

**Problem:** Calculate the magnitude of the electric force and gravitational force between an electron and a proton in a hydrogen atom ($r \approx 5.3 \times 10^{-11}\text{ m}$). What is the ratio $F_e/F_g$?

**Solution:**
This problem demonstrates why physicists entirely ignore gravity when studying subatomic particles. We will calculate both forces using their respective inverse-square laws.

**1. Electric Force ($F_e$):**
Using Coulomb's Law, where $e$ is the elementary charge ($1.6 \times 10^{-19}\text{ C}$):
$$F_e = k \frac{|q_e q_p|}{r^2} = k \frac{e^2}{r^2}$$
$$F_e = (8.99 \times 10^9) \frac{(1.6 \times 10^{-19})^2}{(5.3 \times 10^{-11})^2}$$
$$F_e \approx 8.2 \times 10^{-8}\text{ N}$$

**2. Gravitational Force ($F_g$):**
Using Newton's Law of Universal Gravitation, where $G$ is the gravitational constant ($6.674 \times 10^{-11}\text{ N}\cdot\text{m}^2/\text{kg}^2$), $m_e$ is the electron mass, and $m_p$ is the proton mass:
$$F_g = G \frac{m_e m_p}{r^2}$$
$$F_g = (6.674 \times 10^{-11}) \frac{(9.11 \times 10^{-31})(1.67 \times 10^{-27})}{(5.3 \times 10^{-11})^2}$$
$$F_g \approx 3.6 \times 10^{-47}\text{ N}$$

**3. The Ratio:**
To see how many times stronger the electric force is compared to gravity, we divide the two:
$$\frac{F_e}{F_g} = \frac{8.2 \times 10^{-8}}{3.6 \times 10^{-47}} \approx 2.3 \times 10^{39}$$

The electrostatic attraction holding the atom together is roughly $2.3 \times 10^{39}$ times stronger than the gravitational attraction. Gravity is completely negligible at this scale.

---

## 5. Field Levitation

**Problem:** What electric field strength is required to make a proton levitate against Earth's gravity at the surface? 

**Solution:**
To make a particle levitate, the net force in the vertical direction must be zero. If we draw a free-body diagram of the proton:
1. **Gravity ($F_g$)** pulls down towards the center of the Earth.
2. **The Electric Force ($F_e$)** must push directly upwards to counteract gravity.

Therefore, we can set the magnitudes of these two forces equal to each other:
$$F_e = F_g$$

We know that the electric force on a charge $q$ in an electric field $E$ is $F_e = qE$, and the gravitational force on a mass $m$ is $F_g = mg$. Substituting these in:
$$qE = mg$$

Now, solve for the required electric field strength $E$:
$$E = \frac{mg}{q}$$

Plug in the standard values for a proton ($m_p = 1.67 \times 10^{-27}\text{ kg}$, $q = 1.6 \times 10^{-19}\text{ C}$, and $g = 9.8\text{ m/s}^2$):
$$E = \frac{(1.67 \times 10^{-27}\text{ kg})(9.8\text{ m/s}^2)}{1.6 \times 10^{-19}\text{ C}}$$
$$E \approx 1.02 \times 10^{-7}\text{ V/m}$$

**Direction:** Because a proton has a *positive* charge, it experiences an electric force in the same direction as the electric field lines. Since we need the force to point straight up, the electric field must also point **straight up**.

---

## 6. Field at a point from a system of charges

**Problem:** Two point charges are given: $+q$ at point $(-a, 0)$ and $+2q$ at point $(a, 0)$. Determine various field vectors and limits.

**Solution:**

**1. General Electric Field Vectors:**
The total electric field at any point $(x, y)$ is the vector sum of the fields from each charge: $\vec{E} = \vec{E}_1 + \vec{E}_2$. 
The vector from the first charge to point $(x,y)$ is $\vec{r}_1 = (x+a)\hat{i} + y\hat{j}$. 
The vector from the second charge to point $(x,y)$ is $\vec{r}_2 = (x-a)\hat{i} + y\hat{j}$.

Using $\vec{E} = k \frac{q}{r^2} \hat{r} = k \frac{q}{r^3} \vec{r}$, the general field equation is:
$$\vec{E}(x,y) = k q \left[ \frac{(x+a)\hat{i} + y\hat{j}}{((x+a)^2 + y^2)^{3/2}} \right] + 2k q \left[ \frac{(x-a)\hat{i} + y\hat{j}}{((x-a)^2 + y^2)^{3/2}} \right]$$

To find the field strictly on the y-axis, we plug in $x = 0$:
$$\vec{E}(0,y) = \frac{k q}{(a^2+y^2)^{3/2}} (a\hat{i} + y\hat{j}) + \frac{2k q}{(a^2+y^2)^{3/2}} (-a\hat{i} + y\hat{j})$$
Combine the $\hat{i}$ and $\hat{j}$ terms:
$$\vec{E}(0,y) = \frac{k q}{(a^2+y^2)^{3/2}} (-a\hat{i} + 3y\hat{j})$$

To find the field strictly on the x-axis, we plug in $y = 0$:
$$\vec{E}(x,0) = k q \left[ \frac{\text{sgn}(x+a)}{(x+a)^2} \hat{i} + \frac{2\text{sgn}(x-a)}{(x-a)^2} \hat{i} \right]$$
*(Note: The sign function accounts for whether the test point is to the left or right of the respective charges).*

**2. Condition for Zero Components:**
* **$E_y = 0$:** Looking at the general equation, the $\hat{j}$ component only contains $y$ in the numerator. Therefore, the y-component of the field is only zero on the x-axis ($y = 0$).
* **$E_x = 0$ (and $\vec{E} = 0$):** Since $E_y = 0$ on the x-axis, a true zero field ($\vec{E} = 0$) can only exist on the x-axis. Because both charges are positive, the zero point must lie *between* them ($-a < x < a$), where their field vectors point in opposite directions.
    Setting the magnitudes equal:
    $$\frac{k q}{(x+a)^2} = \frac{2k q}{(a-x)^2}$$
    $$(a-x)^2 = 2(x+a)^2 \implies a-x = \pm\sqrt{2}(x+a)$$
    Solving for the root that lies between the charges yields:
    $$x = a(-3 + 2\sqrt{2}) \approx -0.17a$$

**3. Specific Calculation ($a=0.2$, $y=0.3$, $q=2\mu\text{C}$):**
Since we are evaluating a point on the y-axis, we use the $\vec{E}(0,y)$ equation derived in step 1.
$$\vec{E}(0, 0.3) = \frac{(8.99 \times 10^9)(2 \times 10^{-6})}{(0.2^2 + 0.3^2)^{3/2}} (-0.2\hat{i} + 3(0.3)\hat{j})$$
Calculate the scalar multiplier first: $(0.2^2 + 0.3^2)^{3/2} = (0.13)^{3/2} \approx 0.0468$
$$\text{Scalar factor} = \frac{17980}{0.0468} \approx 3.84 \times 10^5$$
$$\vec{E}(0, 0.3) \approx 3.84 \times 10^5 (-0.2\hat{i} + 0.9\hat{j})\text{ V/m}$$
Distributing the scalar:
$$\vec{E} = (-7.68 \times 10^4 \hat{i} + 3.46 \times 10^5 \hat{j})\text{ V/m}$$

**4. Limit $y \gg a$:**
If we zoom very far out along the y-axis, the distance $y$ becomes overwhelmingly larger than the separation distance $a$. Mathematically, $(a^2 + y^2) \approx y^2$. The $\hat{i}$ components caused by the lateral offset $a$ become negligible compared to the massive vertical distance.
$$\vec{E}(0, y) \approx \frac{kq}{(y^2)^{3/2}}(3y\hat{j}) = \frac{3kq}{y^3}(y\hat{j}) = \frac{3kq}{y^2}\hat{j}$$
**Physical intuition:** From a great distance, the spatial separation of the charges blurs, and the system acts indistinguishably from a single, unified point charge of magnitude $+3q$ located at the origin.

---

## 7. Cyclotron Motion

**Problem:** An electron is accelerated from rest through a potential difference of $5000\text{ V}$. It then enters a region of uniform magnetic field $B = 0.1\text{ T}$, perpendicular to its velocity. What is the radius of the circular path it will follow?

**Solution:**
This problem happens in two distinct stages.

**Stage 1: Electrical Acceleration**
The electron starts at rest and is accelerated by an electric potential. According to the Work-Energy Theorem, the electrical work done on the electron converts entirely into its kinetic energy:
$$W = \Delta K$$
$$qV = \frac{1}{2} m v^2$$
We rearrange this to solve for the final velocity $v$ before it enters the magnetic field:
$$v = \sqrt{\frac{2 q V}{m}}$$
Using the charge ($1.6 \times 10^{-19}\text{ C}$) and mass ($9.11 \times 10^{-31}\text{ kg}$) of an electron:
$$v = \sqrt{\frac{2(1.6 \times 10^{-19}\text{ C})(5000\text{ V})}{9.11 \times 10^{-31}\text{ kg}}} \approx 4.19 \times 10^7\text{ m/s}$$

**Stage 2: Magnetic Deflection**
When the charged particle enters the magnetic field perpendicularly, the magnetic Lorentz force ($F_B = qvB$) acts perpendicular to its velocity. A force that is constantly perpendicular to velocity does no work (doesn't change speed) but continuously changes direction, resulting in uniform circular motion. Therefore, the magnetic force acts as the centripetal force ($F_c = mv^2/r$):
$$F_B = F_c$$
$$q v B = \frac{m v^2}{r}$$

Cancel one $v$ from both sides and solve for the radius $r$:
$$r = \frac{m v}{q B}$$
$$r = \frac{(9.11 \times 10^{-31}\text{ kg})(4.19 \times 10^7\text{ m/s})}{(1.6 \times 10^{-19}\text{ C})(0.1\text{ T})}$$
$$r \approx 2.38 \times 10^{-3}\text{ m}$$

The electron will follow a tight circular path with a radius of **$2.38\text{ mm}$**.

---

## 8. Lorentz Force

**Problem:** A charged particle with charge $q = 2 \times 10^{-19}\text{ C}$ and mass $m = 4 \times 10^{-27}\text{ kg}$ enters a magnetic field of $B = 0.5\text{ T}$ at a speed of $v = 10^6\text{ m/s}$ perpendicular to the field. What is the magnitude of the Lorentz force acting on the particle?

**Solution:**
The magnetic component of the Lorentz force is given by the cross product: $\vec{F} = q(\vec{v} \times \vec{B})$.
When we only care about the *magnitude* of this force, we can use the formula:
$$F = q v B \sin(\theta)$$
where $\theta$ is the angle between the velocity vector and the magnetic field lines. 

Because the problem explicitly states the particle enters "perpendicular to the field," we know that $\theta = 90^\circ$. Since $\sin(90^\circ) = 1$, the formula simplifies to its maximum possible value:
$$F = q v B$$

Now, we just substitute the given values:
$$F = (2 \times 10^{-19}\text{ C}) \cdot (10^6\text{ m/s}) \cdot (0.5\text{ T})$$
$$F = 1.0 \times 10^{-13}\text{ N}$$

The magnitude of the Lorentz force is $1.0 \times 10^{-13}\text{ Newtons}$. *(Note: The mass of the particle is extra information not required to find the force, though it would be needed if you were asked for the resulting acceleration).*

---

## 9. Vector Lorentz Force

**Problem:** A proton moves with a velocity $\vec{v} = (2\hat{i} - 4\hat{j} + \hat{k})\text{ m/s}$ in a region where the magnetic field is $\vec{B} = (\hat{i} + 2\hat{j} - \hat{k})\text{ T}$. What is the magnitude of the magnetic force this charge experiences?

**Solution:**
Because the velocity and magnetic field are given in 3D unit vector notation, we must find the force using the full cross-product definition of the Lorentz force:
$$\vec{F} = q(\vec{v} \times \vec{B})$$

First, let's compute the cross product $\vec{v} \times \vec{B}$ using a matrix determinant. We place the unit vectors in the top row, the velocity components in the middle row, and the magnetic field components in the bottom row:
$$\vec{v} \times \vec{B} = \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ 2 & -4 & 1 \\ 1 & 2 & -1 \end{vmatrix}$$

To expand this determinant, we calculate the $2 \times 2$ sub-determinants for each unit vector. Remember that the $\hat{j}$ term is always subtracted:
$$\vec{v} \times \vec{B} = \hat{i}\begin{vmatrix} -4 & 1 \\ 2 & -1 \end{vmatrix} - \hat{j}\begin{vmatrix} 2 & 1 \\ 1 & -1 \end{vmatrix} + \hat{k}\begin{vmatrix} 2 & -4 \\ 1 & 2 \end{vmatrix}$$

Evaluate each sub-matrix ($ad - bc$):
$$\vec{v} \times \vec{B} = \hat{i}((-4)(-1) - (1)(2)) - \hat{j}((2)(-1) - (1)(1)) + \hat{k}((2)(2) - (-4)(1))$$
$$\vec{v} \times \vec{B} = \hat{i}(4 - 2) - \hat{j}(-2 - 1) + \hat{k}(4 - (-4))$$
$$\vec{v} \times \vec{B} = 2\hat{i} + 3\hat{j} + 8\hat{k}$$

This vector represents $(\vec{v} \times \vec{B})$. Next, we need the *magnitude* of this vector, which we find using the 3D Pythagorean theorem:
$$|\vec{v} \times \vec{B}| = \sqrt{x^2 + y^2 + z^2} = \sqrt{2^2 + 3^2 + 8^2}$$
$$|\vec{v} \times \vec{B}| = \sqrt{4 + 9 + 64} = \sqrt{77} \approx 8.775\text{ m}\cdot\text{T/s}$$

Finally, to get the magnitude of the force, we multiply by the charge of a proton ($q = 1.6 \times 10^{-19}\text{ C}$):
$$F = q|\vec{v} \times \vec{B}| = (1.6 \times 10^{-19}\text{ C}) \cdot \sqrt{77}$$
$$F \approx 1.4 \times 10^{-18}\text{ N}$$

---

## 10. Lorentz Force acting on Wire

**Problem:** A straight wire $2.0\text{ m}$ long carries a current of $10\text{ A}$. It is placed in a uniform magnetic field of $B = 0.5\text{ T}$. Calculate the magnetic force on the wire if the angle between the wire and the magnetic field is: $90^\circ$, $45^\circ$, and $0^\circ$.

**Solution:**
A current-carrying wire in a magnetic field experiences a macroscopic version of the Lorentz force (often called Ampère's Force Law). The magnitude of this force depends on the current $I$, the length of the wire inside the field $L$, the magnetic field strength $B$, and the angle $\theta$ between the direction of the current and the direction of the magnetic field lines.
The formula is:
$$F = I L B \sin(\theta)$$

Before calculating for specific angles, let's calculate the maximum possible force ($ILB$), which acts as our baseline scalar multiplier:
$$F_{\text{max}} = (10\text{ A}) \cdot (2.0\text{ m}) \cdot (0.5\text{ T}) = 10\text{ N}$$

Now we evaluate the force for the given orientations:

**a) Angle is $90^\circ$ (Perpendicular)**
When the wire crosses the field lines at a right angle, it cuts across the maximum number of field lines, resulting in the maximum possible force.
$$F = 10 \cdot \sin(90^\circ) = 10 \cdot (1) = 10\text{ N}$$

**b) Angle is $45^\circ$ (Diagonal)**
When the wire is tilted, only the perpendicular component of the field exerts a force on the charges moving through the wire.
$$F = 10 \cdot \sin(45^\circ) = 10 \cdot \left(\frac{\sqrt{2}}{2}\right) = 5\sqrt{2} \approx 7.07\text{ N}$$

**c) Angle is $0^\circ$ (Parallel)**
When the wire is perfectly parallel to the magnetic field lines, the charges are moving in the exact same direction as the field. Therefore, they do not cross any field lines, and the magnetic field exerts zero force on them.
$$F = 10 \cdot \sin(0^\circ) = 10 \cdot (0) = 0\text{ N}$$