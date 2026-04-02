## 12. Work and Energy with a Constant Force: Step-by-Step

Based on the provided equations, we can establish the following initial conditions and constants for this 2D vector system:
* **Mass ($m$):** 2 kg
* **Constant Force ($\vec{F}$):** $[6, 2] \text{ N}$
* **Initial Velocity ($\vec{v}_0$):** $[1, -1] \text{ m/s}$ (deduced from the velocity equation)
* **Initial Position ($\vec{r}_0$):** $[0, 0] \text{ m}$ (deduced from the position equation)

---

### Step 1: Calculate Acceleration ($\vec{a}$)
Using Newton's Second Law ($\vec{F} = m\vec{a}$), we divide the force vector by the mass to find the constant acceleration:

$$\vec{a} = \frac{\vec{F}}{m}$$
$$\vec{a} = \left[\frac{6}{2}, \frac{2}{2}\right]$$
$$\vec{a} = [3, 1] \text{ m/s}^2$$

---

### Step 2: Formulate Velocity ($\vec{v}(t)$)
Velocity is given by the kinematic equation $\vec{v}(t) = \vec{v}_0 + \vec{a}t$. Substituting our known vectors:

$$\vec{v}(t) = [1, -1] + [3, 1]t$$
$$\vec{v}(t) = [3t + 1, t - 1] \text{ m/s}$$

---

### Step 3: Formulate Position ($\vec{r}(t)$)
Position is given by the kinematic equation $\vec{r}(t) = \vec{r}_0 + \vec{v}_0t + \frac{1}{2}\vec{a}t^2$. Substituting our known vectors:

$$\vec{r}(t) = [0, 0] + [1, -1]t + \frac{1}{2}[3, 1]t^2$$
$$\vec{r}(t) = \left[\frac{3}{2}t^2 + t, \frac{1}{2}t^2 - t\right] \text{ m}$$

---

### Step 4: Calculate Work Done ($W$) at $t = 3$
Work is the dot product of the force vector and the displacement vector ($\Delta\vec{r}$). 
First, find the displacement at $t = 3$ seconds by plugging $t = 3$ into the position equation:

$$\Delta\vec{r}(3) = \left[\frac{3}{2}(3)^2 + 3, \frac{1}{2}(3)^2 - 3\right]$$
$$\Delta\vec{r}(3) = \left[\frac{27}{2} + 3, \frac{9}{2} - 3\right]$$
$$\Delta\vec{r}(3) = [13.5 + 3, 4.5 - 3]$$
$$\Delta\vec{r}(3) = [16.5, 1.5] \text{ m}$$

Now, calculate the work using the dot product ($W = \vec{F} \cdot \Delta\vec{r}$):

$$W = (6 \cdot 16.5) + (2 \cdot 1.5)$$
$$W = 99 + 3$$
$$W = 102 \text{ J}$$

---

### Step 5: Verify with the Work-Energy Theorem
The Work-Energy Theorem states that the work done on an object equals its change in kinetic energy ($W = \Delta KE$). Let's verify this.

$$\Delta KE = \frac{1}{2}m(v_f^2 - v_i^2)$$

First, find the square of the initial velocity magnitude ($v_i^2$):
$$v_i^2 = (1)^2 + (-1)^2 = 1 + 1 = 2$$

Next, find the final velocity vector at $t = 3$ seconds using the velocity equation from Step 2:
$$\vec{v}(3) = [3(3) + 1, (3) - 1] = [10, 2] \text{ m/s}$$

Find the square of the final velocity magnitude ($v_f^2$):
$$v_f^2 = (10)^2 + (2)^2 = 100 + 4 = 104$$

Now, calculate the change in kinetic energy:
$$\Delta KE = \frac{1}{2}(2)(104 - 2)$$
$$\Delta KE = 1(102)$$
$$\Delta KE = 102 \text{ J}$$

**Conclusion:** The work calculated directly from the force and displacement ($102 \text{ J}$) exactly matches the change in kinetic energy ($102 \text{ J}$), confirming our results are perfectly consistent with the Work-Energy Theorem!