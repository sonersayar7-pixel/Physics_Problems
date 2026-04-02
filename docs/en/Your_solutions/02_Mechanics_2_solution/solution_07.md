## 7. Dynamics with Friction: Step-by-Step

Based on the problem description, we have a **10 kg** block being pulled, with a **5 kg** block sitting on top of it. The top block is tied down, meaning it slides against the bottom block as the bottom block moves. 

Here are our given variables:
* **Mass of bottom block ($M$):** **10 kg**
* **Mass of top block ($m$):** **5 kg**
* **Applied force ($F$):** **45 N**
* **Coefficient of kinetic friction ($\mu$):** **0.2**
* **Acceleration due to gravity ($g$):** **9.8 m/s²**

---

### Step 1: Calculate friction from the top block ($f_2$)
Because the top block is tied, it drags against the bottom block ($M$). The normal force for this interaction is just the weight of the top block ($mg$). The friction force $f_2$ resisting the motion of $M$ is:

$$f_2 = \mu mg$$

Substitute the known values:

$$f_2 = 0.2 \cdot 5 \cdot 9.8$$
$$f_2 = 9.8 \text{ N}$$

---

### Step 2: Calculate friction from the ground ($f_1$)
The ground supports both blocks, so the normal force here is the combined weight of both masses $(m + M)g$. The friction force $f_1$ from the ground resisting the motion of $M$ is:

$$f_1 = \mu (m + M)g$$

Substitute the known values (total mass = **15 kg**):

$$f_1 = 0.2 \cdot (5 + 10) \cdot 9.8$$
$$f_1 = 0.2 \cdot 15 \cdot 9.8$$
$$f_1 = 29.4 \text{ N}$$

---

### Step 3: Calculate the net force ($\sum F$)
The net force acting on the bottom block ($M$) is the forward applied force ($F$) minus the two resistive friction forces ($f_1$ and $f_2$):

$$\sum F = F - f_1 - f_2$$

Substitute the calculated values:

$$\sum F = 45 - 29.4 - 9.8$$
$$\sum F = 5.8 \text{ N}$$

---

### Step 4: Calculate the acceleration ($a$)
Using Newton's Second Law ($\sum F = Ma$), we can find the acceleration of the bottom block. Note that we only use the mass of the bottom block ($M = 10 \text{ kg}$) because it is the only object actually moving.

$$a = \frac{\sum F}{M}$$

Substitute the values:

$$a = \frac{5.8}{10}$$
$$a = 0.58 \text{ m/s}^2$$

**Final Answer:** The net force acting on the bottom block is **5.8 N**, resulting in an acceleration of **0.58 m/s²**.