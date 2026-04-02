## 8. Work of a Variable Force: Step-by-Step

This problem explores the relationship between force, work, and potential energy in a spring system (a simple harmonic oscillator) where the force is not constant, but instead varies with position.

---

### Step 1: The Equation of Motion
According to Hooke's Law, the restoring force of an ideal spring is proportional to its displacement: $F = -kx$. 
Using Newton's Second Law ($F = ma$, where acceleration $a$ is the second derivative of position with respect to time), we can write this as a differential equation:

$$m\frac{d^2x}{dt^2} = -kx$$

The general solution to this differential equation describes the object's position over time:

$$x(t) = A\cos(\omega t + \phi)$$

Where the angular frequency $\omega$ is defined as:

$$\omega = \sqrt{\frac{k}{m}}$$

---

### Step 2: Calculate the Work Done ($W$)
Because the force changes continuously as the object moves, we must use integration to calculate the work done by the spring force as the object is displaced from equilibrium ($x = 0$) to a specific position ($x_0$). 

The formula for work is the integral of force over distance:

$$W = \int_{0}^{x_0} F(x) \, dx$$

Substitute the spring force $F(x) = -kx$ into the integral:

$$W = \int_{0}^{x_0} -kx \, dx$$

Apply the power rule for integration:

$$W = \left[ -\frac{1}{2}kx^2 \right]_{0}^{x_0}$$

Evaluate the definite integral from the bounds $0$ to $x_0$:

$$W = -\frac{1}{2}kx_0^2 - \left(-\frac{1}{2}k(0)^2\right)$$
$$W = -\frac{1}{2}kx_0^2$$

---

### Step 3: Determine the Potential Energy ($U$)
For a conservative force like a spring, the potential energy function $U(x)$ is defined as the negative of the work done by the force to reach that position ($U = -W$). 

Assuming the potential energy at equilibrium is zero, the potential energy at any given position $x$ is:

$$U(x) = -W$$

Substitute the expression for work we calculated in Step 2:

$$U(x) = -\left(-\frac{1}{2}kx^2\right)$$
$$U(x) = \frac{1}{2}kx^2$$

---

### Step 4: Verification
We can verify that our potential energy equation is correct by working backward. A fundamental property of conservative forces is that the force is the negative spatial derivative of the potential energy:

$$F = -\frac{dU}{dx}$$

Take the derivative of our potential energy equation $U(x) = \frac{1}{2}kx^2$ with respect to $x$:

$$-\frac{dU}{dx} = -\frac{d}{dx}\left(\frac{1}{2}kx^2\right)$$

Apply the power rule for derivatives (multiply by the exponent $2$, then reduce the exponent by $1$):

$$-\frac{dU}{dx} = -\left(2 \cdot \frac{1}{2}kx^1\right)$$
$$-\frac{dU}{dx} = -kx$$

This perfectly matches our original force equation $F = -kx$, successfully verifying our work!