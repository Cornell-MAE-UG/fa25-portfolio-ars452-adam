---
layout: project
title: Thermodynamic Analysis of the Cummins X12 Engine
description: An analysis of the MCI J4500 bus engine cycle efficiency and power output under varying weather conditions.
image: assets/images/X12_engine_photo.png
category: [Thermodynamics]
---

Earlier this week, after completing my last final of the Fall 2025, I scurried home to leave behind all of my semester blues. The journey from Ithaca to my home in NYC was fortunately made smooth and efficient thanks to Cornell's Campus to Campus shuttle service, which provides round-trip service between the university's medical and general campuses. The shuttle service primarily utilizes the MCI J4500 motorcoach, so as a way to give thanks for the impeccable transportation, I have chosen to analyze the engine that powers this incredible bus.

## Background

The MCI J4500 is among the best-selling motor coaches in the United States, praised for its for dependability and comfort across uses ranging from intercity travel to tour operations. The **Cummins X12** is the heavy-duty diesel engine behind this beauty, renowened for its high power-to-weight ratio that makes operating (and resting in) the bus a seamless experience.

<img src="../../assets/images/C2Cbus.jpg" width=500px>

The Cummins X12 in this application produces up to 455 HP and utilizes a 4-stroke compression-ignition cycle. To fully analyze its thermodynamics properties, I will:

1.  Calculate the Diesel Cycle efficiency, Power, and MEP of the X12 assuming room temperature intake conditions (intercooled).
2.  Recalculate these values assuming 0°C (273 K) operating conditions, simulating winter driving (as is typical in the depths of Ithaca's winter).
3.  Compare the ideal thermodynamic performance to the real-world rated power.

## Engine Specifications and Assumptions

**Cummins X12 Specifications:**

* **Compression ratio ($r$):** 18.3:1
* **Engine displacement ($V_{total}$):** 11.9 Liters ($0.0119 \text{ m}^3$)
* **Cylinders:** 6 (Inline)
* **Displacement per cylinder ($V_d$):** 1.98 Liters ($0.00198 \text{ m}^3$)
* **Rated Power:** 455 HP at 1800 RPM

**Analysis Assumptions:**

Let's then define some assumptions that can make this analysis more palatable:

* **Model:** Cold-air-standard **Diesel Cycle** (Isobaric Heat Addition).
* **Intake Pressure ($P_1$):** 200 kPa (Assumed boost pressure from turbocharger).
* **Combustion Input ($q_{in}$):** $1.8 \times 10^6 \text{ J/kg}$ (Estimate for full-load diesel combustion).
* **Specific Heats:** Constant specific heats for air ($\gamma = 1.4$, $c_p = 1005 \text{ J/kg K}$, $c_v = 718 \text{ J/kg K}$).
* **Processes:** Adiabatic compression/expansion, Isobaric heat addition, Isochoric heat rejection.

## Real vs. Idealized Cycles

A real diesel cycle involves complex injection timing and blowdown phases. However, we can model it thermodynamically as the Ideal Diesel Cycle consisting of the following four processes:

1.  **Isentropic Compression (1 → 2)**
2.  **Isobaric Heat Addition (2 → 3)** (Fuel injection and combustion)
3.  **Isentropic Expansion (3 → 4)** (Power stroke)
4.  **Isochoric Heat Rejection (4 → 1)** (Exhaust)

The Ideal Diesel Cycle can be modeled on PV and TS diagrams, as drawn below. Notice how process 2-3 is constant pressure and process 4-1 is constant volume.

<img src="../../assets/images/C2Cbus.jpg" width=500px>

This cycle also provides the upper bound for the engine's efficiency and power output, which is what we can use for subsequent calucations.

## Performance Calculations

This analysis evaluates the ideal Diesel cycle performance of one cylinder of the Cummins X12. The total engine power will be 6 times the single-cylinder output (since the engine contains 6 cylinders, all assumed to function similar thermodynamically).

**Inputs:**

$$
T_1 = 300\ \text{K}, \quad r = 18.3, \quad \gamma = 1.4
$$
$$
P_1 = 200\ \text{kPa}, \quad R = 287\ \text{J/kg K}, \quad V_d = 1.98\times10^{-3}\ \text{m}^3 (displacment volume)
$$
$$
q_{in} = 1.8 \times 10^6\ \text{J/kg}
$$

### 1. Compression Process (1 → 2)

**Assumption:** Adiabatic and reversible compression.

$$
T_2 = T_1 r^{\gamma-1} = 300 \cdot 18.3^{0.4} = 960\ \text{K}
$$

$$
P_2 = P_1 r^{\gamma} = 200 \cdot 18.3^{1.4} = 11,740\ \text{kPa} = 11.74\ \text{MPa}
$$

**Cylinder Volumes:**

$$
V_1 = V_d \frac{r}{r-1} = 1.98\times10^{-3} \left(\frac{18.3}{17.3}\right) = 2.09\times10^{-3}\ \text{m}^3
$$

$$
V_2 = \frac{V_1}{r} = 1.14\times10^{-4}\ \text{m}^3
$$

This is the volume that they cylinder compresses to from stage 1 to 2.
### 2. Heat Addition (2 → 3)

**Assumption:** Isobaric heat addition (Constant Pressure).

$$
P_3 = P_2 = 11.74\ \text{MPa}
$$

$$
T_3 = T_2 + \frac{q_{in}}{c_p} = 960 + \frac{1.8\times10^6}{1005} = 2751\ \text{K}
$$

We calculate the **Cutoff Ratio ($r_c$)**:

$$
r_c = \frac{T_3}{T_2} = \frac{2751}{960} = 2.87
$$

### 3. Expansion (3 → 4)

**Assumption:** Isentropic expansion. The effective expansion ratio is $r/r_c$.

$$
T_4 = T_3 \left(\frac{r_c}{r}\right)^{\gamma-1} = 2751 \left(\frac{2.87}{18.3}\right)^{0.4} = 1313\ \text{K}
$$

$$
P_4 = P_3 \left(\frac{r_c}{r}\right)^{\gamma} = 11.74 \left(\frac{2.87}{18.3}\right)^{1.4} = 0.86\ \text{MPa}
$$

$$
q_{out} = c_v(T_4 - T_1) = 718(1313 - 300) = 7.27\times10^{5}\ \text{J/kg}
$$

### 4. Cycle Efficiency and Work

$$
w_{net} = q_{in} - q_{out} = 1.8\times10^6 - 7.27\times10^5 = 1.073\times10^{6}\ \text{J/kg}
$$

$$
\eta = \frac{w_{net}}{q_{in}} = \frac{1.073}{1.8} = 0.596 = 59.6\%
$$

### 5. Mass per Cycle and Work Output

**Assumption:** Ideal gas law at state 1.

$$
m = \frac{P_1 V_1}{R T_1} = \frac{200,000 \cdot 2.09\times10^{-3}}{287 \cdot 300} = 4.85\times10^{-3}\ \text{kg}
$$

$$
W_{\text{cyl}} = m \cdot w_{net} = (4.85\times10^{-3}) (1.073\times10^6) = 5204\ \text{J}
$$

$$
\text{MEP} = \frac{W_{\text{cyl}}}{V_d} = \frac{5204}{1.98\times10^{-3}} = 2.63\ \text{MPa}
$$

**Total Power Output ($P_{ind}$):**
At 1800 RPM (30 rev/sec), with 6 cylinders, and 1 power stroke per 2 revs:

$$
P_{total} = W_{\text{cyl}} \cdot (\text{Cylinders}) \cdot \frac{\text{RPM}}{60 \cdot 2}
$$

$$
P_{total} = 5204 \cdot 6 \cdot \frac{1800}{120} = 468,360\ \text{W} = 468.4\ \text{kW} \approx 628\ \text{HP}
$$

Comparing to the real life Cummins X12 power output of 455 HP:

$$
\mu_{\text{real}} = \frac{455}{628} \approx 72.5\%
$$

#### Summary of Results (Room Temp.)

$$
\eta = 59.6\%, \quad \text{MEP} = 2.63\ \text{MPa}, \quad \mu_{\text{real}} \approx 72.5\%
$$

---

## Performance Calculations (0°C Intake Temperature)

This second analysis simulates driving the MCI J4500 in winter conditions (0°C). Cold air is denser, increasing the mass of air in the cylinder, which should theoretically increase power output if the turbocharger maintains the same boost pressure.

**New Intake Temperature:**
$$
T_1 = 273\ \text{K} \quad (0^\circ\text{C})
$$

We assume the same boost pressure ($P_1 = 200 \text{ kPa}$) and slightly adjusted specific heats for colder air ($\gamma \approx 1.4$, assumed constant for comparison).

### 1. Compression Process (1 → 2)

$$
T_2 = 273 \cdot 18.3^{0.4} = 874\ \text{K}
$$

$$
P_2 = 200 \cdot 18.3^{1.4} = 11.74\ \text{MPa}
$$
Volumes $V_1$ and $V_2$ remain unchanged.

### 2. Heat Addition (2 → 3)

We keep $q_{in}$ constant ($1.8 \text{ MJ/kg}$).

$$
T_3 = 874 + \frac{1.8\times10^6}{1005} = 2665\ \text{K}
$$

$$
r_c = \frac{2665}{874} = 3.05
$$

### 3. Expansion Process (3 → 4)

$$
T_4 = 2665 \left(\frac{3.05}{18.3}\right)^{0.4} = 1302\ \text{K}
$$

$$
P_4 = 11.74 \left(\frac{3.05}{18.3}\right)^{1.4} = 0.95\ \text{MPa}
$$

$$
q_{out} = 718(1302 - 273) = 7.39\times10^{5}\ \text{J/kg}
$$

### 4. Cycle Efficiency and Work

$$
w_{net} = 1.8\times10^6 - 7.39\times10^5 = 1.061\times10^{6}\ \text{J/kg}
$$

$$
\eta = \frac{1.061}{1.8} = 0.589 = 58.9\%
$$
*(Note: Efficiency drops slightly. In the Diesel cycle, a higher cutoff ratio $r_c$ reduces thermal efficiency. Since the colder air resulted in a higher $r_c$ for the same energy input, efficiency decreased slightly).*

### 5. Mass per Cycle and Work Output

$$
m = \frac{P_1 V_1}{R T_1} = \frac{200,000 \cdot 2.09\times10^{-3}}{287 \cdot 273} = 5.33\times10^{-3}\ \text{kg}
$$

$$
W_{\text{cyl}} = (5.33\times10^{-3})(1.061\times10^6) = 5655\ \text{J}
$$

$$
\text{MEP} = \frac{5655}{1.98\times10^{-3}} = 2.85\ \text{MPa}
$$

$$
P_{total} = 5655 \cdot 6 \cdot \frac{1800}{120} = 508,950\ \text{W} \approx 682\ \text{HP}
$$

Comparing to real output (assuming real output scales similarly, or utilizing the higher potential):

$$
\mu_{\text{real-cold}} = \frac{455}{682} \approx 66.7\%
$$

## Summary of Results (0°C)

$$
\eta = 58.9\%, \quad \text{MEP} = 2.85\ \text{MPa}, \quad P_{ideal} \approx 682\ \text{HP}
$$

## Comparisons / Conclusions

The analysis of the Cummins X12 reveals that:

1.  **Efficiency:** The Diesel efficiency is high (~60%), but interestingly, it decreased slightly (by 0.7%) in the cold air scenario. This is because the denser cold air required a longer isobaric expansion (higher cutoff ratio) to absorb the same specific heat input, which is thermodynamically less efficient than isochoric heat addition.
2.  **Power:** Despite the slight efficiency drop, the power output significalty increased  (from 628 HP to 682 HP, a measurable 8.6% increase). This is driven purely by the increased air density ($m$ increased), allowing more working fluid to process the energy per cycle.
3.  **Real vs. Ideal:** The engine operates at about 72.5% of its theoretical air-standard limit. The remaining losses are due to friction, heat transfer to coolant, pumping losses (turbo backpressure), and non-instantaneous combustion (irreversibilities).

This explains why buses like the J4500 can feel more "peppy" in the winter; the engine is breathing denser air, producing more torque and power, even if the thermodynamic efficiency cycle-to-cycle is marginally lower.

**Technologies Used:** Hand calculations, Goodnotes

<script>
  MathJax = {
    tex: {
      inlineMath: [['$', '$'], ['\\(', '\\)']],
      displayMath: [['$$', '$$'], ['\\[', '\\]']]
    }
  };
</script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js"></script>
