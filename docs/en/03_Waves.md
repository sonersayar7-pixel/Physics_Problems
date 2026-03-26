# Section 3: Waves - Solutions

## 1. Wave Properties
The relationship between speed ($v$), frequency ($f$), and wavelength ($\lambda$) is given by $v = f\lambda$.
* **In Air:**
  $$\lambda_{air} = \frac{v_{air}}{f} = \frac{343 \text{ m/s}}{440 \text{ Hz}} \approx 0.78 \text{ m}$$
* **In Water:**
  $$\lambda_{water} = \frac{v_{water}}{f} = \frac{1482 \text{ m/s}}{440 \text{ Hz}} \approx 3.37 \text{ m}$$

---

## 2. String Harmonics
For the fundamental frequency ($n=1$) of a string fixed at both ends, the length $L$ is half a wavelength: $L = \lambda/2 \implies \lambda = 2L$.

$$L = 64 \text{ cm} = 0.64 \text{ m} \implies \lambda = 1.28 \text{ m}$$
$$v = f\lambda = 330 \text{ Hz} \times 1.28 \text{ m} = 422.4 \text{ m/s}$$

---

## 3. Superposition Principle
Using the trigonometric identity $\sin(A) + \sin(B) = 2 \sin(\frac{A+B}{2}) \cos(\frac{A-B}{2})$:
$$y_{res} = A[\sin(kx - \omega t) + \sin(kx + \omega t)] = 2A \sin(kx) \cos(\omega t)$$
* **Nodes:** Occur where the spatial part is zero: $\sin(kx) = 0$.
  $$kx = n\pi \implies x = \frac{n\pi}{k} = \frac{n\lambda}{2} \quad \text{for } n = 0, 1, 2, \dots$$

---

## 4. Phase Difference
The phase difference $\Delta \phi$ is related to path difference $\Delta x$ by $\Delta \phi = \frac{2\pi}{\lambda} \Delta x$.
$$\Delta \phi = \frac{2\pi}{\lambda} \left( \frac{\lambda}{3} \right) = \frac{2\pi}{3} \text{ radians (or } 120^\circ)$$

---

## 5. Echo Ranging
The sound travels to the cliff and back, covering a distance of $2d$ in time $t$.
$$2d = v \cdot t \implies d = \frac{343 \text{ m/s} \times 1 \text{ s}}{2} = 171.5 \text{ m}$$

---

## 6. Wave Equation
$y(x,t) = 0.05 \sin(2\pi x - 50\pi t)$. Compare to $y = A \sin(kx - \omega t)$:
* **a) Amplitude:** $A = 0.05 \text{ m}$.
* **b) Wavelength:** $k = 2\pi \implies \frac{2\pi}{\lambda} = 2\pi \implies \lambda = 1 \text{ m}$.
* **c) Frequency:** $\omega = 50\pi \implies 2\pi f = 50\pi \implies f = 25 \text{ Hz}$.
* **d) Wave Speed:** $v = f\lambda = 25 \times 1 = 25 \text{ m/s}$ (or $v = \omega/k$).

---

## 7. Standing Wave Modes
For a string of length $L$, the wavelength of the $n$-th harmonic (where $n$ is the number of antinodes) is $\lambda_n = \frac{2L}{n}$.

$$\lambda = \frac{2 \times 80 \text{ cm}}{4} = 40 \text{ cm} = 0.4 \text{ m}$$

---

## 8. Traveling Wave Functions
A function $f(x,t)$ describes a traveling wave if it is of the form $f(x \pm vt)$.
* **a) $A \cos(kx^2 - \omega t)$:** No. The $x^2$ term prevents it from being in the form $(x-vt)$.
* **b) $A(x-vt)^2$:** **Yes.** It is a function of $(x-vt)$ and satisfies the wave equation.
* **c) $A \log(x+vt)$:** **Yes.** It is a function of $(x+vt)$ and satisfies the wave equation.

---

## 9. Damped Oscillator
The equation is $m \ddot{x} + b \dot{x} + kx = 0$. Let $\gamma = \frac{b}{2m}$ and $\omega_0 = \sqrt{\frac{k}{m}}$.

1. **General Solution:** $x(t) = e^{-\gamma t}(C_1 e^{\sqrt{\gamma^2 - \omega_0^2}t} + C_2 e^{-\sqrt{\gamma^2 - \omega_0^2}t})$.
2. **Classification:**
   * **Underdamped ($\gamma < \omega_0$):** Oscillates with decaying amplitude.
   * **Critically Damped ($\gamma = \omega_0$):** Returns to equilibrium fastest without oscillation.
   * **Overdamped ($\gamma > \omega_0$):** Returns to equilibrium slowly without oscillation.

---

## 10. Animation: Wave Sources
The intensity of the wave follows an inverse power law $1/r^\alpha$.
* If $\alpha = 0$: Plane waves (no attenuation).
* If $\alpha = 0.5$: Cylindrical waves.
* If $\alpha = 1.0$: Spherical waves (standard 3D point source).
The resultant displacement at any point $\vec{r}$ is:
$$U_{total}(\vec{r},t) = \sum_{i} \frac{A}{|\vec{r}-\vec{r_i}|^\alpha} \sin(k |\vec{r} - \vec{r_i}| - \omega t)$$

---

## 11. Animation: Two-Slit Interference
The interference pattern is governed by the path difference $\Delta r = |\vec{r}-\vec{r_1}| - |\vec{r}-\vec{r_2}|$.

* **Constructive interference:** $\Delta r = n\lambda$.
* **Destructive interference:** $\Delta r = (n + \frac{1}{2})\lambda$.
Increasing $d$ (slit distance) results in closer interference fringes, while increasing $\lambda$ (wavelength) spreads the fringes further apart.