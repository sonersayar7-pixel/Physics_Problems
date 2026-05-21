### 1. Propagation of Error I: Volume of a Sphere

**Given:**

* Radius: $r$ = 6.20 cm
* Absolute uncertainty: $\Delta r$ = 0.05 cm

**Step 1: Calculate the Nominal Volume ($V$)**
The volume of a sphere is given by the formula:


$$V = \frac{4}{3}\pi r^3$$


Substituting the given radius:


$$V = \frac{4}{3}\pi (6.20\text{ cm})^3$$

$$V \approx 998.31\text{ cm}^3$$

**Step 2: Calculate the Propagated Uncertainty ($\Delta V$)**
Using the power rule for fractional uncertainties:


$$\frac{\Delta V}{V} = 3 \left( \frac{\Delta r}{r} \right)$$


Isolating the absolute uncertainty $\Delta V$:


$$\Delta V = V \cdot 3 \left( \frac{\Delta r}{r} \right)$$

$$\Delta V = 998.31\text{ cm}^3 \cdot 3 \left( \frac{0.05\text{ cm}}{6.20\text{ cm}} \right)$$

$$\Delta V \approx 24.15\text{ cm}^3$$

**Final Result:**


$$V = (998 \pm 24)\text{ cm}^3$$

---

### 2. Propagation of Error II: Area of a Rectangular Plate

**Given:**

* Length: $L$ = 15.3 cm, with $\Delta L$ = 0.1 cm
* Width: $W$ = 8.4 cm, with $\Delta W$ = 0.1 cm

**Step 1: Calculate the Nominal Area ($A$)**


$$A = L \cdot W$$

$$A = 15.3\text{ cm} \cdot 8.4\text{ cm}$$

$$A = 128.52\text{ cm}^2$$

**Step 2: Calculate the Propagated Uncertainty ($\Delta A$) via Quadrature**
For independent random uncertainties in multiplication:


$$\frac{\Delta A}{A} = \sqrt{\left(\frac{\Delta L}{L}\right)^2 + \left(\frac{\Delta W}{W}\right)^2}$$


Isolating $\Delta A$:


$$\Delta A = A \cdot \sqrt{\left(\frac{\Delta L}{L}\right)^2 + \left(\frac{\Delta W}{W}\right)^2}$$

$$\Delta A = 128.52\text{ cm}^2 \cdot \sqrt{\left(\frac{0.1}{15.3}\right)^2 + \left(\frac{0.1}{8.4}\right)^2}$$

$$\Delta A = 128.52 \cdot \sqrt{0.0000427 + 0.0001417}$$

$$\Delta A = 128.52 \cdot 0.01358 \approx 1.74\text{ cm}^2$$

**Final Result:**


$$A = (128.5 \pm 1.7)\text{ cm}^2$$

---

### 3. Propagation of Error III: Ohm's Law

**Given:**

* Voltage: $V$ = 10.0 V, with $\Delta V$ = 0.2 V
* Current: $I$ = 2.00 A, with $\Delta I$ = 0.05 A

**Step 1: Calculate the Nominal Resistance ($R$)**


$$R = \frac{V}{I}$$

$$R = \frac{10.0\text{ V}}{2.00\text{ A}}$$

$$R = 5.00\text{ }\Omega$$

**Step 2: Calculate the Propagated Uncertainty ($\Delta R$)**
Using the standard addition of relative errors for division:


$$\frac{\Delta R}{R} = \frac{\Delta V}{V} + \frac{\Delta I}{I}$$


Isolating $\Delta R$:


$$\Delta R = R \cdot \left( \frac{\Delta V}{V} + \frac{\Delta I}{I} \right)$$

$$\Delta R = 5.00\text{ }\Omega \cdot \left( \frac{0.2\text{ V}}{10.0\text{ V}} + \frac{0.05\text{ A}}{2.00\text{ A}} \right)$$

$$\Delta R = 5.00 \cdot (0.02 + 0.025)$$

$$\Delta R = 5.00 \cdot 0.045 = 0.225\text{ }\Omega$$

**Final Result:**


$$R = (5.00 \pm 0.23)\text{ }\Omega$$

---

### 4. Relative Uncertainty

**Given:**

* Speedometer reading: $v$ = 60 km/h
* Relative uncertainty: **5%**

**Step 1: Calculate the Absolute Uncertainty ($\Delta v$)**


$$\Delta v = v \cdot 5\%$$

$$\Delta v = 60\text{ km/h} \cdot 0.05$$

$$\Delta v = 3\text{ km/h}$$

**Step 2: Determine the Actual Speed Range**


$$\text{Range} = [v - \Delta v, v + \Delta v]$$

$$\text{Range} = [60 - 3, 60 + 3]\text{ km/h}$$

$$\text{Range} = [57, 63]\text{ km/h}$$

---

### 5. Percentage Calculation

**Given:**

* Time measurement: $t$ = 5.45 s
* Absolute uncertainty: $\Delta t$ = 0.22 s

**Step 1: Calculate Percentage Uncertainty**


$$\text{Percentage Uncertainty} = \left( \frac{\Delta t}{t} \right) \cdot 100\%$$

$$\text{Percentage Uncertainty} = \left( \frac{0.22\text{ s}}{5.45\text{ s}} \right) \cdot 100\%$$

$$\text{Percentage Uncertainty} \approx 4.04\%$$

---

### 6. Instrument Precision

**Given:**

* Thermometer reading: $T$ = 25.4°C

**Step 1: Identify the Value of the Last Digit**
The last recorded digit is in the tenths place:
**Last Digit Value = 0.1°C**

**Step 2: Apply the Uncertainty Rule**
The absolute uncertainty $\Delta T$ is half the value of the last digit:


$$\Delta T = \frac{0.1^\circ\text{C}}{2}$$

$$\Delta T = 0.05^\circ\text{C}$$

---

### 7. Standard Deviation

**Given Sample Dataset** ($N$ = 11):


$$x = \{88, 92, 79, 85, 95, 81, 86, 90, 83, 77, 89\}$$

#### Part A: Computation for the Complete Set ($N$ = 11)

**Step 1: Compute the Mean ($\bar{x}$)**


$$\bar{x} = \frac{1}{N} \sum_{i=1}^N x_i$$

$$\bar{x} = \frac{88 + 92 + 79 + 85 + 95 + 81 + 86 + 90 + 83 + 77 + 89}{11}$$

$$\bar{x} = \frac{945}{11} \approx 85.91$$

**Step 2: Compute the Sample Standard Deviation ($\sigma$)**


$$\sigma = \sqrt{\frac{1}{N-1} \sum_{i=1}^N (x_i - \bar{x})^2}$$

$$\sum_{i=1}^{11} (x_i - 85.91)^2 \approx 310.91$$

$$\sigma = \sqrt{\frac{310.91}{11 - 1}} = \sqrt{31.091} \approx 5.58$$

#### Part B: Computation with Extremes Removed ($N$ = 9)

We remove the highest value (**95**) and lowest value (**77**).


$$x_{\text{new}} = \{88, 92, 79, 85, 81, 86, 90, 83, 89\}$$

**Step 1: Compute the New Mean ($\bar{x}_{\text{new}}$)**


$$\bar{x}_{\text{new}} = \frac{88 + 92 + 79 + 85 + 81 + 86 + 90 + 83 + 89}{9}$$

$$\bar{x}_{\text{new}} = \frac{773}{9} \approx 85.89$$

**Step 2: Compute the New Sample Standard Deviation ($\sigma_{\text{new}}$)**


$$\sum_{i=1}^{9} (x_i - 85.89)^2 \approx 148.89$$

$$\sigma_{\text{new}} = \sqrt{\frac{148.89}{9 - 1}} = \sqrt{18.611} \approx 4.31$$

---

### 8. Mass-Spring Measurements: Analytical Formulas

When evaluating data collected from your mass-spring simulation setup, the governing mathematical relationships for analysis are modeled as follows:

**Step 1: Mean Period ($T$) and Period Uncertainty ($\Delta T$)**
Let $t_{\text{total}}$ be the measured time for **10** oscillations. The period $T$ for a single oscillation is:


$$T = \frac{\bar{t}_{\text{total}}}{10}$$


The uncertainty of the period corresponds to the sample standard deviation of your experimental runs:


$$\Delta T = \sigma_T$$

**Step 2: Calculate the Spring Constant ($k$)**
From the dynamic definition of a simple harmonic oscillator ($T = 2\pi\sqrt{\frac{m}{k}}$):


$$k = \frac{4\pi^2 m}{T^2}$$

**Step 3: Propagate the Uncertainty of the Spring Constant ($\Delta k$)**
Assuming mass $m$ has zero uncertainty ($\Delta m$ = 0):


$$\frac{\Delta k}{k} = 2 \left( \frac{\Delta T}{T} \right)$$

$$\Delta k = k \cdot 2 \left( \frac{\Delta T}{T} \right)$$

---

### 9. Pendulum Measurements: Analytical Formulas

For analyzing data derived from either the manual HTML stopwatch pendulum tool or your physical real-world pendulum experiment, use the equations derived below:

**Step 1: Determine Single Oscillation Period ($T$)**


$$T = \frac{\bar{t}_{\text{10 oscillations}}}{10}$$

**Step 2: Calculate the Acceleration Due to Gravity ($g$)**
Squaring the standard period relation ($T = 2\pi\sqrt{\frac{L}{g}}$) and solving for $g$:


$$g = \frac{4\pi^2 L}{T^2}$$

**Step 3: Propagate the Uncertainty of Gravity ($\Delta g$)**
Assuming the pendulum length $L$ is treated as an exact value ($\Delta L$ = 0):


$$\frac{\Delta g}{g} = 2 \left( \frac{\Delta T}{T} \right)$$

$$\Delta g = g \cdot 2 \left( \frac{\Delta T}{T} \right)$$

---

### 10. Light Speed Measurement

**Experimental Framework:**

* Microwave Frequency: $f$ = 2.45 GHz = $2.45 \cdot 10^9$ Hz
* Measured distance between adjacent melted spots: $d$ = 6.0 cm = 0.06 m

**Step 1: Determine the Wavelength ($\lambda$)**
Because hotspots form at standing wave antinodes, the distance between adjacent spots represents a half-wavelength ($\frac{\lambda}{2}$):


$$\lambda = 2 \cdot d$$

$$\lambda = 2 \cdot 0.06\text{ m} = 0.12\text{ m}$$

**Step 2: Calculate the Experimental Speed of Light ($c_{\text{measured}}$)**
Using the fundamental wave speed equation:


$$c_{\text{measured}} = f \cdot \lambda$$

$$c_{\text{measured}} = (2.45 \cdot 10^9\text{ Hz}) \cdot (0.12\text{ m})$$

$$c_{\text{measured}} = 2.94 \cdot 10^8\text{ m/s}$$

**Step 3: Calculate the Percentage Error**
Given the standard accepted value $c_{\text{accepted}}$ = $3.00 \cdot 10^8$ m/s:


$$\text{Percentage Error} = \left( \frac{|c_{\text{measured}} - c_{\text{accepted}}|}{c_{\text{accepted}}} \right) \cdot 100\%$$

$$\text{Percentage Error} = \left( \frac{|2.94 \cdot 10^8\text{ m/s} - 3.00 \cdot 10^8\text{ m/s}|}{3.00 \cdot 10^8\text{ m/s}} \right) \cdot 100\%$$

$$\text{Percentage Error} = \left( \frac{6.00 \cdot 10^6}{3.00 \cdot 10^8} \right) \cdot 100\% = 2\%$$