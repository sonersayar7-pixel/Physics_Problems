# Physics Study Guide: Circuit Analysis & Electromagnetism

This repository contains step-by-step solutions for circuit reduction, Kirchhoff's Laws, and electromagnetic theory.

---

## 1. Fundamental Series and Parallel Circuits
**Goal:** Calculate equivalent resistance ($$R_{eq}$$) and total current ($$I$$).

**Step 1: Series Analysis**
In a series circuit, charge has only one path. The resistances add directly.


[Image of series and parallel resistor circuits]

- Formula: $$R_{series} = \sum R_i$$
- Calculation: $$15 + 30 + 50 = 95\,\Omega$$
- Current ($$V=IR$$): $$I = 12 / 95 \approx 0.126\,\text{A}$$

**Step 2: Parallel Analysis**
In parallel, the voltage is the same across all branches, but the current splits.
- Formula: $$\frac{1}{R_{parallel}} = \sum \frac{1}{R_i}$$
- Calculation: $$\frac{1}{15} + \frac{1}{30} + \frac{1}{50} = 0.12\,\Omega^{-1}$$
- Invert for result: $$R_{eq} = \frac{1}{0.12} = 8.33\,\Omega$$
- Total Current: $$I = 12 / 8.33 \approx 1.44\,\text{A}$$

---

## 2. Resistor Permutations (Three 1-Ohm Resistors)
**Goal:** Find all unique total resistance values possible using exactly three identical resistors.

1. **Maximum Resistance (All Series):** $$1 + 1 + 1 = 3\,\Omega$$
2. **Minimum Resistance (All Parallel):** $$\frac{1}{1+1+1} = 0.33\,\Omega$$
3. **Hybrid A (Two in series, then parallel with one):** $$\frac{2 \times 1}{2 + 1} = 0.67\,\Omega$$
4. **Hybrid B (Two in parallel, then series with one):** $$0.5 + 1 = 1.5\,\Omega$$

---

## 3. Complex Network Reduction (r1)
**Goal:** Solve for $$R_{eq}$$when$$R = 5\,\Omega$$.

**Step 1: Identify Sub-circuits.** We look for the "innermost" components first.
- The top branch has two resistors in series: $$R_a = 5 + 5 = 10\,\Omega$$.
- The bottom branch has a parallel pair ($$5 || 5 = 2.5\,\Omega$$) in series with a $$5\,\Omega$$resistor:$$R_b = 5 + 2.5 = 7.5\,\Omega$$.

**Step 2: Combine Branches.**
These two branches ($$10\,\Omega$$and$$7.5\,\Omega$$) are in parallel.
- $$R_{parallel} = \frac{10 \times 7.5}{10 + 7.5} = 4.29\,\Omega$$

**Step 3: Final Series.**
Add the final resistor at the entrance of the circuit:
- $$R_{total} = 4.29 + 5 = 9.29\,\Omega$$

---

## 4. Bridge Circuit Analysis (r2)
**Goal:** Solve for $$R_{eq}$$for the grid (all$$R = 10\,\Omega$$).



[Image of a resistor bridge circuit]

This circuit represents a **Symmetrical Bridge**. 
- Because the resistance values are identical on all sides, the potential difference across the center vertical resistor is zero. 
- No current flows through the center. We can remove it mentally.
- This leaves two parallel branches, each consisting of two $$10\,\Omega$$ resistors in series ($$20\,\Omega$$ each).
- $$R_{eq} = \frac{20 \times 20}{20 + 20} = 10\,\Omega$$

---

## 5. Kirchhoff’s Loop Rules (k1)
**Goal:** Find the current in each branch.



[Image of Kirchhoff's voltage and current laws]

**Step 1: Junction Rule.**
At the center node: $$I_1 + I_3 = I_2$$.

**Step 2: Voltage Loops.**
- **Left Loop:** $$4.5 - I_1(20 + 1) - I_2(10) = 0$$
- **Right Loop:** $$9 - I_3(1) - I_2(10) = 0$$

**Step 3: Substitution.**
Solving the system of linear equations yields:
- $$I_1 = -0.167\,\text{A}$$ (The negative sign means the actual current flows opposite to our assumed arrow).
- $$I_2 = 0.803\,\text{A}$$
- $$I_3 = 0.971\,\text{A}$$

---

## 6. Nodal Analysis (k2)
**Goal:** Find the current through the ammeter in the middle branch.

**Step 1: Define a Node.** Let the top node be $$V$$ and the bottom be ground ($$0\,\text{V}$$).
**Step 2: KCL Equation.**
The sum of currents leaving node $$V$$ must be zero:
$$\frac{V - 9}{10} + \frac{V - 0}{20} + \frac{V - 4.5}{10} = 0$$

**Step 3: Solve for V.**
Multiply the whole equation by 20:
$$2(V-9) + V + 2(V-4.5) = 0$$
$$5V - 27 = 0 \implies V = 5.4\,\text{V}$$

**Step 4: Ammeter Current.**
$$I = \frac{5.4}{20} = 0.27\,\text{A}$$

---

## 7. Capacitor Energy and Charge
**Goal:** Calculate total charge and energy for $$4\,\mu\text{F}$$and$$6\,\mu\text{F}$$ in parallel.

- **Equivalent Capacitance:** $$C_{eq} = 4 + 6 = 10\,\mu\text{F}$$
- **Total Charge:** $$Q = CV = (10 \times 10^{-6}) \times 10 = 100\,\mu\text{C}$$
- **Energy Stored:** $$U = \frac{1}{2}CV^2 = 0.5 \times (10 \times 10^{-6}) \times 100 = 5 \times 10^{-4}\,\text{J}$$

---

## 8. AC Voltage Signal
**Goal:** Convert current $$I(t) = 2 \sin(120\pi t)$$to Voltage for$$R = 50\,\Omega$$.

By Ohm's Law: $$V(t) = I(t) \times R$$
$$V(t) = [2 \sin(120\pi t)] \times 50 = 100 \sin(120\pi t)\,\text{V}$$

---

## 9. Calculus of Current
**Goal:** Find current at $$t = 3\,\text{s}$$given$$Q(t) = 5t^2 + 5$$.

- **Instantaneous Current:** $$I(t) = \frac{dQ}{dt}$$
- **Derivative:** $$10t$$
- **At t = 3:** $$10 \times 3 = 30\,\text{A}$$

---

## 10. Lightning Bolt (Average Current)
**Goal:** Find $$I_{avg}$$for$$30\,\text{C}$$in$$2\,\text{ms}$$.

- **Conversion:** $$2\,\text{ms} = 0.002\,\text{s}$$
- **Formula:** $$I = \frac{\Delta Q}{\Delta t} = \frac{30}{0.002} = 15,000\,\text{A}$$

---

## 11. Household Power and Energy
**Goal:** Find Power and Energy for a $$100\,\Omega$$resistor at$$50\,\text{V}$$ for 5 minutes.

- **Power:** $$P = \frac{V^2}{R} = \frac{2500}{100} = 25\,\text{W}$$
- **Energy:** $$E = P \times t = 25 \times (5 \times 60) = 7,500\,\text{J}$$

---

## 12. Ideal Transformers
**Goal:** Find secondary voltage and primary current.



[Image of a transformer step-down and step-up]

- **Voltage Ratio:** $$V_s = V_p \left( \frac{N_s}{N_p} \right) = 120 \times \left( \frac{200}{1000} \right) = 24\,\text{V}$$
- **Current Ratio (Inverse):** $$I_p = I_s \left( \frac{V_s}{V_p} \right) = 3 \times \left( \frac{24}{120} \right) = 0.6\,\text{A}$$

---

## 13. Winding Ratio
**Goal:** Find $$N_s$$to drop$$120\,\text{V}$$to$$9\,\text{V}$$.

$$\frac{N_s}{N_p} = \frac{V_s}{V_p} \implies N_s = 400 \times \left( \frac{9}{120} \right) = 30\,\text{turns}$$

---

## 14. The RLC Analogy
**Goal:** Compare electrical circuits to mechanical oscillators.


The differential equation for an RLC circuit is:
$$L \frac{d^2q}{dt^2} + R \frac{dq}{dt} + \frac{1}{C}q = V(t)$$

**Physical Mappings:**
- **Inductance ($$L$$) = Mass ($$m$$):** Both represent inertia (resistance to change).
- **Resistance ($$R$$) = Damping ($$b$$):** Both dissipate energy as heat.
- **Inverse Capacitance ($$1/C$$) = Spring Constant ($$k$$):** Both represent potential energy storage.

---

## 15. The Resistor Cube
**Goal:** Find equivalent resistance across the main diagonal.

This is solved using **symmetry**. When current enters a corner, it splits into 3 identical edges ($$R/3$$ resistance). It then splits into 6 edges ($$R/6$$ resistance), and finally converges into 3 edges ($$R/3$$ resistance).
- Total Resistance: $$\frac{1}{3}R + \frac{1}{6}R + \frac{1}{3}R = \frac{5}{6}R \approx 0.833R$$