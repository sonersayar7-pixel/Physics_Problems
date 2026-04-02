## 9. Vertical Throw with Drag: Step-by-Step

This problem models an object thrown straight upward while experiencing linear air resistance (drag). We will find its velocity over time and analyze its maximum height.

---

### Step 1: Set up the differential equation
Using Newton's Second Law ($F_{net} = ma$), we sum the downward forces acting on the object (gravity and air drag). Defining upward as the positive direction:

$$m\frac{dv}{dt} = -mg - kv$$

Divide by mass ($m$) and factor out a negative sign to isolate the derivative:

$$\frac{dv}{dt} = -\left(g + \frac{k}{m}v\right)$$

---

### Step 2: Separate variables and integrate
Group the velocity ($v$) terms on one side and time ($t$) on the other:

$$\frac{dv}{g + \frac{k}{m}v} = -dt$$

Integrate both sides (from initial velocity $v_0$ to $v(t)$, and time $0$ to $t$):

$$\int_{v_0}^{v(t)} \frac{1}{g + \frac{k}{m}v} \, dv = \int_{0}^{t} -dt$$

Evaluating this integral (using the natural logarithm) and solving for $v(t)$ yields the velocity function:

$$v(t) = \left(v_0 + \frac{mg}{k}\right)e^{-\frac{k}{m}t} - \frac{mg}{k}$$

---

### Step 3: Determine the condition for Maximum Height
The object reaches its maximum peak height at the exact moment it stops moving upward and is about to fall back down. This occurs when the velocity is zero:

$$v(t) = 0$$

You can set the velocity equation from Step 2 to $0$ and solve for $t$ to find the exact time it takes to reach this peak. 

---

### Step 4: Compare with the Vacuum Case
In a perfect vacuum (where $k = 0$, meaning no air resistance), mechanical energy is fully conserved. The maximum height in a vacuum is derived purely from kinematic equations:

$$h_{vacuum} = \frac{v_0^2}{2g}$$

**Conclusion:** When drag is introduced, the maximum height reached by the object will always be **lower** than the vacuum case ($h_{drag} < h_{vacuum}$). This happens because the drag force continuously performs negative work on the object, dissipating its initial kinetic energy into the surrounding air as heat and fluid displacement before it can be fully converted into gravitational potential energy.