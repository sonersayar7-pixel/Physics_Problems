## 10. Animation and Simulation: Multiple Wave Sources

When programming animations or physical simulations (like ripples in a pond or acoustics in a room), we often need to calculate the behavior of waves spreading out from multiple points at once. As a wave travels outward from its source, its energy spreads over a larger area, causing its amplitude to decrease (attenuate) over distance. 



### Step 1: The Power Law of Attenuation
The way a wave's amplitude drops as it moves away from the source follows an inverse power law. The geometry of the wave determines the exponent ($\alpha$) in the denominator.

Let $r$ be the distance from the source. The amplitude drops by a factor of $\frac{1}{r^\alpha}$:

* **Plane Waves ($\alpha = 0$):** The amplitude does not decrease with distance ($1/r^0 = 1$). This models a massive, flat wave front (like a laser beam or distant ocean swells) moving in a single direction without spreading.
* **Cylindrical Waves ($\alpha = 0.5$):** The amplitude drops by $\frac{1}{\sqrt{r}}$. This models waves spreading out in 2D space, such as dropping a pebble into a flat pool of water.
* **Spherical Waves ($\alpha = 1.0$):** The amplitude drops by $\frac{1}{r}$. This models waves spreading out in all directions in 3D space, like a star emitting light or a firecracker exploding in the air. *(Note: Because intensity is amplitude squared, this results in the famous $1/r^2$ inverse-square law for intensity!)*

---

### Step 2: The Master Displacement Equation
To find the total displacement ($U_{total}$) at any specific point in space ($\vec{r}$) at any given time ($t$), we must add up the contributions of *all* the individual wave sources. We use this master summation equation:

$$U_{total}(\vec{r},t) = \sum_{i} \frac{A}{|\vec{r}-\vec{r_i}|^\alpha} \sin(k |\vec{r} - \vec{r_i}| - \omega t)$$

Let's break down the anatomy of this equation:

* **The Superposition ($\sum_i$):** The summation symbol tells us to calculate the wave from source 1, source 2, source 3, etc., and add them all together algebraically.
* **The Distance ($|\vec{r} - \vec{r_i}|$):** This represents the physical, straight-line distance from the $i$-th wave source ($\vec{r_i}$) to the point we are observing ($\vec{r}$).
* **The Attenuation Term ($\frac{A}{|\dots|^\alpha}$):** The original amplitude ($A$) divided by the distance raised to our geometric factor ($\alpha$). This ensures the wave gets mathematically weaker the further away the observation point is from the source.
* **The Traveling Wave Phase ($\sin(k |\dots| - \omega t)$):** This is our familiar traveling wave function! The distance $|\vec{r} - \vec{r_i}|$ acts as our "$x$" variable, allowing the wave to propagate outward from the source point over time $t$.

### Conclusion for Presentation
This equation is the ultimate engine for wave simulations. By simply feeding a computer a list of source locations ($\vec{r_i}$), a standard amplitude ($A$), and choosing whether the world is 2D ($\alpha=0.5$) or 3D ($\alpha=1.0$), the program can use this single formula to render complex, overlapping wave interference patterns in real-time.