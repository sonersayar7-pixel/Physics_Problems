## Section 10: 3D Kinematic Analysis (Elliptical Helix)

**Position Vector:** $\vec{r}(t) = (a \cos\omega t, b \sin\omega t, bt)$

### 1. Trajectory Equation
The projection on the $xy$-plane follows:
$$\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1$$
In 3D space, this represents an **elliptical helix** climbing the $z$-axis.

### 2. Path Length Integral
The instantaneous speed is:
$$v(t) = \sqrt{a^2\omega^2 \sin^2(\omega t) + b^2\omega^2 \cos^2(\omega t) + b^2}$$
Total distance $s$ for $t \in [0, t_0]$:
$$s = \int_{0}^{t_0} v(t) \, dt$$

### 3. Special Case: Circular Helix ($a=b$)
If the semi-axes are equal, the speed is constant, and the length simplifies to:
$$s = b t_0 \sqrt{\omega^2 + 1}$$