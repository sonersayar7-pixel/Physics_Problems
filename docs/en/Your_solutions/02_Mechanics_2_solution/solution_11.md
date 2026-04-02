## 11. Dynamics with a Time-Dependent Force: Step-by-Step

This problem involves finding an object's velocity and position over time by integrating a time-dependent acceleration vector. 

Based on the final equations provided, we can deduce the initial conditions (constants of integration) at $t = 0$:
* **Initial Velocity ($\vec{v}_0$):** $(2, 0, 1) \text{ m/s}$
* **Initial Position ($\vec{r}_0$):** $(5, 2, -3) \text{ m}$

---

### Step 1: Define the Acceleration ($\vec{a}$)
Using Newton's Second Law ($\vec{a} = \frac{\vec{F}}{m}$), the problem provides the resulting acceleration vector as a function of time:

$$\vec{a}(t) = (5t, t - 4, -2t^2)$$

---

### Step 2: Calculate the Velocity ($\vec{v}$)
Velocity is the integral of acceleration with respect to time. To find the velocity vector, we integrate each component of the acceleration vector and add the initial velocity vector $\vec{v}_0$:

$$\vec{v}(t) = \int \vec{a}(t) \, dt + \vec{v}_0$$

Integrate the components:
* **X-component:** $\int 5t \, dt = \frac{5}{2}t^2$
* **Y-component:** $\int (t - 4) \, dt = \frac{1}{2}t^2 - 4t$
* **Z-component:** $\int -2t^2 \, dt = -\frac{2}{3}t^3$

Now, add the initial velocity constants $\vec{v}_0 = (2, 0, 1)$:

$$\vec{v}(t) = \left(\frac{5}{2}t^2 + 2, \frac{1}{2}t^2 - 4t + 0, -\frac{2}{3}t^3 + 1\right)$$

Simplify to get the final velocity vector:

$$\vec{v}(t) = \left(\frac{5}{2}t^2 + 2, \frac{1}{2}t^2 - 4t, -\frac{2}{3}t^3 + 1\right)$$

---

### Step 3: Calculate the Position ($\vec{r}$)
Position is the integral of velocity with respect to time. To find the position vector, we integrate each component of our newly found velocity vector and add the initial position vector $\vec{r}_0$:

$$\vec{r}(t) = \int \vec{v}(t) \, dt + \vec{r}_0$$

Integrate the components:
* **X-component:** $\int (\frac{5}{2}t^2 + 2) \, dt = \frac{5}{6}t^3 + 2t$
* **Y-component:** $\int (\frac{1}{2}t^2 - 4t) \, dt = \frac{1}{6}t^3 - 2t^2$
* **Z-component:** $\int (-\frac{2}{3}t^3 + 1) \, dt = -\frac{1}{6}t^4 + t$

Now, add the initial position constants $\vec{r}_0 = (5, 2, -3)$:

$$\vec{r}(t) = \left(\frac{5}{6}t^3 + 2t + 5, \frac{1}{6}t^3 - 2t^2 + 2, -\frac{1}{6}t^4 + t - 3\right)$$

**Final Answer:** The velocity vector over time is **$\vec{v}(t) = (\frac{5}{2}t^2 + 2, \frac{1}{2}t^2 - 4t, -\frac{2}{3}t^3 + 1)$**. 
The position vector over time is **$\vec{r}(t) = (\frac{5}{6}t^3 + 2t + 5, \frac{1}{6}t^3 - 2t^2 + 2, -\frac{1}{6}t^4 + t - 3)$**.