## Section 12: Kinematic Path Analysis

**Alice:** $A(t) = (2+t, 8-3t)$  
**Bob:** $B(t) = (2t-1, 2t+2)$

### Intersection vs. Collision
* **Collision:** No. Solving $A(t) = B(t)$ yields inconsistent values for $t$ ($t=3$ vs $t=1.2$).
* **Intersection Point:** Yes. Paths cross at $(2.75, 5.75)$.
  * Alice arrives at $t = 0.75$
  * Bob arrives at $t = 1.875$

### Proximity Analysis
The minimum distance occurs when the derivative of the squared distance function $D^2(t)$ is zero:
$$f(t) = (t-3)^2 + (5t-6)^2 \implies f'(t) = 52t - 66$$
* **Time of closest approach:** $t \approx 1.27 \text{ s}$
* **Minimum Distance:** $D \approx 1.74 \text{ units}$