## Section 9.2: Range Optimization Analysis

To analytically prove that the maximum horizontal range is achieved at a launch angle of $45^\circ$, we must find the extreme value of the range function $R(\theta)$ by evaluating its derivative with respect to $\theta$.

### 1. The Range Function
The horizontal range $R$ of a projectile launched from ground level with initial velocity $v_0$ and angle $\theta$ is given by:
$$R(\theta) = \frac{v_0^2 \sin(2\theta)}{g}$$

### 2. First Derivative Test
To find the maximum value, we take the derivative of $R(\theta)$ with respect to $\theta$ and set it to zero:
$$\frac{dR}{d\theta} = \frac{d}{d\theta} \left[ \frac{v_0^2 \sin(2\theta)}{g} \right]$$

Since $v_0$ and $g$ are constants:
$$\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot \cos(2\theta) \cdot 2$$
$$\frac{dR}{d\theta} = \frac{2v_0^2 \cos(2\theta)}{g}$$

### 3. Solving for Critical Points
Set the derivative to zero to find the stationary point:
$$0 = \frac{2v_0^2 \cos(2\theta)}{g}$$

For this equation to hold true, the cosine term must be zero:
$$\cos(2\theta) = 0$$

The general solution for $\cos(x) = 0$ in the first quadrant is $x = 90^\circ$:
$$2\theta = 90^\circ$$
$$\theta = 45^\circ$$

### 4. Verification (Second Derivative Test)
To confirm this point is a maximum, we evaluate the second derivative $\frac{d^2R}{d\theta^2}$:
$$\frac{d^2R}{d\theta^2} = \frac{d}{d\theta} \left[ \frac{2v_0^2 \cos(2\theta)}{g} \right] = -\frac{4v_0^2 \sin(2\theta)}{g}$$

Substituting $\theta = 45^\circ$:
$$\frac{d^2R}{d\theta^2} = -\frac{4v_0^2 \sin(90^\circ)}{g} = -\frac{4v_0^2}{g}$$

Since the second derivative is negative ($< 0$), the function $R(\theta)$ has a local maximum at $\theta = 45^\circ$.

### Conclusion
The maximum horizontal range is achieved when:
$$\theta_{\text{max}} = 45^\circ$$
At this angle, $\sin(2\theta) = \sin(90^\circ) = 1$, yielding:
$$R_{\text{max}} = \frac{v_0^2}{g}$$