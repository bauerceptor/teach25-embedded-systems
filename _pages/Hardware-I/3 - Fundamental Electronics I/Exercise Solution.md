---
title: "Exercise Solutions - Fundamental Electronics I"
date: "2024-01-01"
thumbnail: "/assets/img/exercise-solutions-bg.jpg"
---

# Exercise Solutions: Chapter 3 - Fundamental Electronics I

*Note: These solutions are provided for practice and understanding. They demonstrate proper application of semiconductor device principles and circuit analysis techniques.*

## Multiple Choice Questions

### Question 1: _____ allows uni-directional flow of current.
**Answer: c. Diode**

**Explanation:** A diode is specifically designed to allow current flow in only one direction (forward bias) while blocking current flow in the reverse direction. This one-way conduction property makes diodes essential for rectification, protection, and switching applications.

### Question 2: _____ is used for load regulation.
**Answer: b. Zener Diode**

**Explanation:** Zener diodes are specifically designed to operate in the reverse breakdown region where they maintain a constant voltage across a wide range of currents. This property makes them ideal for voltage regulation applications where a stable output voltage is required despite variations in input voltage or load current.

### Question 3: _____ can be used as a switch.
**Answer: a. BJT**

**Explanation:** Bipolar Junction Transistors (BJTs) can operate in two distinct modes: cut-off (acting as an open switch) and saturation (acting as a closed switch). This switching capability makes BJTs useful for digital circuits, LED drivers, and power control applications.

### Question 4: There are _____ p-n junctions in a BJT
**Answer: b. 2**

**Explanation:** A BJT consists of three semiconductor regions (either NPN or PNP configuration) which creates two p-n junctions: the emitter-base junction and the base-collector junction. These two junctions work together to provide the transistor's amplification and switching capabilities.

### Question 5: _______ is always used in reverse bias.
**Answer: c. Zener diode**

**Explanation:** Zener diodes are specifically designed to operate in reverse bias mode, particularly in the breakdown region where they maintain a constant voltage. While regular diodes are damaged by reverse breakdown, Zener diodes are manufactured to safely operate in this region for voltage regulation.

---

## Short Answer Questions

### Question 1: Define Diode.

**Answer:** A diode is a two-terminal semiconductor device consisting of a p-n junction that allows current to flow easily in one direction (forward bias) while blocking current flow in the opposite direction (reverse bias). It behaves like an electrical one-way valve, conducting when the anode is positive relative to the cathode, and blocking when the anode is negative relative to the cathode.

### Question 2: What are the applications of diode?

**Answer:** 
- **Rectification:** Converting AC to DC in power supplies
- **Voltage regulation:** Using Zener diodes for stable voltage references
- **Signal detection:** Demodulating AM radio signals
- **Protection circuits:** Preventing reverse polarity damage
- **Switching circuits:** Digital logic and control applications
- **Clipping and clamping:** Signal processing and waveform shaping
- **Frequency multiplication:** Using diode nonlinearity for harmonic generation

### Question 3: Describe the formation of PN junction diode.

**Answer:** A PN junction is formed by joining p-type and n-type semiconductor materials. When these materials come into contact, holes from the p-side diffuse to the n-side while electrons from the n-side diffuse to the p-side due to concentration gradients. This diffusion leaves behind immovable ionized atoms, creating a depletion region with positive charges on the n-side and negative charges on the p-side. An electric field develops across this region, opposing further diffusion. Equilibrium is reached when the diffusion current equals the drift current, resulting in a built-in potential barrier of approximately 0.7V for silicon and 0.3V for germanium.

### Question 4: Define rectification.

**Answer:** Rectification is the process of converting alternating current (AC) to direct current (DC) using diodes. During the positive half-cycle of AC input, the diode conducts and allows current to flow through the load. During the negative half-cycle, the diode blocks current flow. This results in a pulsating DC output that flows in only one direction, though filtering is typically required to smooth the output for practical applications.

### Question 5: Describe Half Wave rectifier.

**Answer:** A half-wave rectifier uses a single diode to rectify AC voltage. During the positive half-cycle of the input AC voltage, the diode is forward-biased and conducts, allowing current to flow through the load resistor. During the negative half-cycle, the diode is reverse-biased and blocks current flow, resulting in no current through the load. The output is a pulsating DC voltage that utilizes only half of the input AC waveform, making it relatively inefficient with about 40.6% efficiency and high ripple content.

### Question 6: Describe Full Wave rectifier.

**Answer:** A full-wave rectifier utilizes both halves of the AC input cycle to produce a more continuous DC output. There are two main types: center-tap and bridge rectifiers. In a center-tap rectifier, two diodes conduct alternately with each half-cycle using a center-tapped transformer. In a bridge rectifier, four diodes are arranged so that two diodes conduct during each half-cycle. Full-wave rectifiers have higher efficiency (about 81.2%), lower ripple content, and better transformer utilization compared to half-wave rectifiers.

### Question 7: Define Zener diode.

**Answer:** A Zener diode is a heavily doped semiconductor diode designed to operate reliably in the reverse breakdown region. Unlike regular diodes that are damaged by reverse breakdown, Zener diodes are manufactured to have a precise breakdown voltage and can safely conduct reverse current when this voltage is exceeded. They maintain an approximately constant voltage across their terminals over a wide range of reverse currents, making them ideal for voltage regulation and reference applications.

---

## Detailed Answer Questions

### Question 1: Describe the formation of zener diode.

**Answer:**

A Zener diode is formed through a specialized manufacturing process that creates a heavily doped p-n junction designed for reliable reverse breakdown operation.

**Manufacturing Process:**

**Heavy Doping:** Both the p-type and n-type regions are heavily doped with impurities at much higher concentrations than regular diodes. The p-region is heavily doped with acceptor atoms (like boron), while the n-region is heavily doped with donor atoms (like phosphorus or arsenic).

**Thin Depletion Region:** The heavy doping creates a very thin depletion region, typically only a few micrometers wide. This thin region is crucial for the Zener effect to occur at relatively low voltages.

**Controlled Breakdown Voltage:** The doping concentration and profile are precisely controlled during manufacturing to achieve a specific breakdown voltage. Different doping levels produce Zener diodes with breakdown voltages ranging from 2.4V to over 200V.

**Crystal Structure:** The semiconductor crystal structure is optimized to ensure uniform electric field distribution across the junction, enabling consistent breakdown characteristics.

**Physical Construction:** The device is constructed with appropriate electrode contacts and packaging to handle the power dissipation during reverse breakdown operation.

**Breakdown Mechanisms:**

**Zener Effect (Low Voltages):** For breakdown voltages below about 6V, the primary mechanism is the Zener effect, where high electric field strength causes direct rupture of covalent bonds, allowing electrons to tunnel through the energy barrier.

**Avalanche Effect (High Voltages):** For breakdown voltages above about 6V, avalanche multiplication becomes dominant. High-energy charge carriers collide with atoms, creating additional electron-hole pairs through impact ionization.

**Temperature Characteristics:** The manufacturing process can be optimized to achieve desired temperature coefficients. Zener effect has a negative temperature coefficient, while avalanche effect has a positive coefficient. Around 6V, both effects balance to create temperature-stable references.

### Question 2: Define load regulation and how zener diode can be used for load regulation.

**Answer:**

**Load Regulation Definition:**

Load regulation is a measure of how well a voltage source maintains a constant output voltage when the load current changes. It is typically expressed as the percentage change in output voltage when the load current varies from minimum to maximum rated values.

Load Regulation = ((VNL - VFL) / VFL) × 100%

Where:
- VNL = No-load voltage (minimum current)
- VFL = Full-load voltage (maximum current)

Good load regulation means the output voltage remains nearly constant regardless of load current variations.

**Zener Diode Load Regulation:**

A Zener diode provides excellent load regulation through its unique reverse breakdown characteristics. When operated in the breakdown region, the Zener diode maintains an approximately constant voltage across its terminals despite significant changes in current.

**Basic Zener Regulator Circuit:**

The circuit consists of:
- Input voltage source (varying DC voltage)
- Series limiting resistor
- Zener diode in reverse bias
- Load resistance (which may vary)

**Regulation Mechanism:**

**Constant Output Voltage:** The Zener diode clamps the output voltage to its breakdown voltage (VZ). As long as the Zener current remains above the knee current, the output voltage stays approximately constant at VZ.

**Current Redistribution:** When load current increases:
1. Total current through the series resistor remains approximately constant
2. Increased load current is compensated by decreased Zener current
3. Output voltage remains stable at VZ

**When load current decreases:**
1. The "extra" current that was previously flowing through the load now flows through the Zener diode
2. Zener current increases to maintain constant total current
3. Output voltage remains stable at VZ

**Design Considerations:**

**Series Resistance Selection:** The series resistor must be chosen to ensure:
- Minimum Zener current flows under maximum load conditions
- Maximum Zener current doesn't exceed power rating under minimum load conditions
- Adequate voltage drop across the resistor for regulation

**Power Dissipation:** Both the Zener diode and series resistor must be rated for maximum expected power dissipation:
- PZ = VZ × IZ(max)
- PR = I² × R

**Regulation Range:** Effective regulation occurs only when the Zener operates in its breakdown region. The circuit cannot regulate if input voltage drops below VZ plus the minimum voltage drop across the series resistor.

**Practical Applications:**
- Computer power supplies for stable logic voltages
- Instrument reference voltages
- Bias voltage generation for amplifiers
- Protection circuits for sensitive components

### Question 3: What is the difference between Silicon and germanium based diodes.

**Answer:**

Silicon and germanium diodes differ significantly in their electrical, thermal, and practical characteristics due to the fundamental properties of these semiconductor materials.

**Electrical Characteristics:**

**Forward Voltage Drop:**
- **Silicon Diodes:** Approximately 0.7V forward voltage drop at room temperature
- **Germanium Diodes:** Approximately 0.3V forward voltage drop at room temperature

This difference affects power dissipation and circuit design considerations.

**Reverse Saturation Current:**
- **Silicon Diodes:** Very low reverse saturation current (nanoamperes to picoamperes)
- **Germanium Diodes:** Higher reverse saturation current (microamperes)

Lower reverse current means better switching characteristics and lower power loss in reverse bias.

**Breakdown Voltage:**
- **Silicon Diodes:** Higher breakdown voltages possible (up to several kilovolts)
- **Germanium Diodes:** Lower breakdown voltages, typically limited to a few hundred volts

**Thermal Characteristics:**

**Operating Temperature Range:**
- **Silicon Diodes:** -65°C to +200°C (excellent high-temperature performance)
- **Germanium Diodes:** -60°C to +100°C (limited by intrinsic carrier generation)

**Temperature Coefficient:**
- **Silicon Diodes:** Forward voltage decreases by about 2mV/°C
- **Germanium Diodes:** Forward voltage decreases by about 2.5mV/°C

**Thermal Runaway:**
- **Silicon Diodes:** More resistant to thermal runaway due to wider bandgap
- **Germanium Diodes:** More susceptible to thermal runaway at elevated temperatures

**Physical Properties:**

**Bandgap Energy:**
- **Silicon:** 1.12 eV (wider bandgap)
- **Germanium:** 0.67 eV (narrower bandgap)

The wider bandgap of silicon provides better temperature stability and higher breakdown voltages.

**Crystal Structure:**
- Both have diamond crystal structure but different lattice constants
- Silicon: 5.43 Å lattice constant
- Germanium: 5.65 Å lattice constant

**Manufacturing and Cost:**

**Availability:**
- **Silicon:** Abundant raw material (silicon dioxide in sand)
- **Germanium:** Relatively rare and expensive element

**Manufacturing Process:**
- **Silicon:** Well-established, high-volume production processes
- **Germanium:** More specialized manufacturing, higher costs

**Processing Temperature:**
- **Silicon:** Higher processing temperatures required
- **Germanium:** Lower processing temperatures sufficient

**Practical Applications:**

**Silicon Diodes - Preferred for:**
- Power applications requiring high temperature operation
- High-voltage applications
- General-purpose rectification
- Integrated circuits and modern electronics
- Applications requiring low reverse leakage current

**Germanium Diodes - Preferred for:**
- Low-voltage applications where 0.3V drop is advantageous
- High-frequency applications (historically)
- Temperature-sensitive applications requiring lower threshold
- Specialized analog circuits requiring soft knee characteristics

**Historical Context:**

**Development Timeline:**
- Germanium diodes were developed first (1940s-1950s)
- Silicon technology matured later but became dominant by 1960s
- Modern electronics predominantly use silicon due to superior characteristics

**Current Usage:**
- Silicon dominates modern electronics (>95% of semiconductor devices)
- Germanium limited to specialized applications
- Compound semiconductors (GaAs, SiC, GaN) used for specific high-performance applications

**Performance Comparison:**

**Switching Speed:**
- Silicon generally faster switching due to lower stored charge
- Germanium can have advantages in some high-frequency applications

**Efficiency:**
- Silicon more efficient in most applications due to lower reverse current
- Germanium may be more efficient in very low voltage applications

**Reliability:**
- Silicon much more reliable, especially at elevated temperatures
- Germanium requires more careful thermal management

**Environmental Stability:**
- Silicon devices more stable over time and environmental conditions
- Germanium more sensitive to contamination and aging effects

---

## Problem Solutions

### Problem 1: Zener Diode Circuit with Two Zeners

**Given:**
- Two Zener diodes in series, each rated at 15V, 200mA
- Input voltage: 45V unregulated supply

**Find:**
(i) The regulated output voltage
(ii) The value of series resistance R

**Solution:**

**(i) Regulated Output Voltage:**

Since the two 15V Zener diodes are connected in series and both operate in breakdown region:

Output voltage = VZ1 + VZ2 = 15V + 15V = **30V**

**(ii) Series Resistance Calculation:**

**Step 1:** Determine operating conditions
- For proper regulation, both Zeners must operate in breakdown region
- Assume load current = 0 for maximum Zener current condition
- Maximum Zener current per diode = 200mA

**Step 2:** Apply KVL around the circuit
Vin = VR + Vout
45V = IR × R + 30V
VR = 45V - 30V = 15V

**Step 3:** Calculate series resistance
For maximum current condition (no load):
R = VR / Imax = 15V / 0.2A = **75Ω**

**Step 4:** Verify power ratings
- Power in each Zener: PZ = 15V × 0.2A = 3W
- Power in resistor: PR = (0.2A)² × 75Ω = 3W

**Answer:** (i) Regulated output voltage = 30V, (ii) Series resistance R = 75Ω

### Problem 2: Variable Load Zener Regulator

**Given:**
- 10V Zener diode for voltage regulation
- Input voltage varies: 13V to 16V
- Load current varies: 10mA to 85mA
- Minimum Zener current: 15mA

**Find:** Value of series resistance R

**Solution:**

**Step 1:** Identify critical conditions
- **Worst case for Zener current:** Maximum input voltage (16V) and minimum load current (10mA)
- **Design condition:** Minimum input voltage (13V) and maximum load current (85mA)

**Step 2:** Apply design condition (minimum Vin, maximum IL)
At minimum input voltage with maximum load current, Zener current should be at minimum value (15mA).

Using KVL: Vin = VR + VZ
13V = IR × R + 10V
VR = 3V

Total current: I = IZ + IL = 15mA + 85mA = 100mA

**Step 3:** Calculate series resistance
R = VR / I = 3V / 0.1A = **30Ω**

**Step 4:** Verify worst-case condition
At maximum input voltage (16V) with minimum load current (10mA):
VR = 16V - 10V = 6V
I = VR / R = 6V / 30Ω = 200mA
IZ = I - IL = 200mA - 10mA = 190mA

This is acceptable if the Zener can handle 190mA.

**Answer:** Series resistance R = 30Ω

### Problem 3: Zener Regulator with Variable Input

**Given:**
- Zener voltage VZ = 18V
- Zener current must be maintained between 200mA and 2A
- Output voltage E0 = 18V
- Input voltage Ei varies: 22V to 28V
- Load current: Not specified (assume variable)

**Find:** Value of series resistance R

**Solution:**

**Step 1:** Establish design constraints
- Minimum Zener current: 200mA (for regulation)
- Maximum Zener current: 2A (for power rating)
- Input voltage range: 22V to 28V

**Step 2:** Determine critical design points

**Case 1 - Minimum input, maximum load:**
When Ei = 22V and Zener current = 200mA (minimum)
VR = Ei - E0 = 22V - 18V = 4V
This represents minimum total current condition.

**Case 2 - Maximum input, minimum load:**
When Ei = 28V and Zener current = 2A (maximum)
VR = Ei - E0 = 28V - 18V = 10V
This represents maximum total current condition.

**Step 3:** Calculate resistance for each case

**For Case 1:**
R1 = VR / Imin = 4V / 0.2A = 20Ω

**For Case 2:**
R2 = VR / Imax = 10V / 2A = 5Ω

**Step 4:** Select appropriate resistance
The series resistance must satisfy both conditions. If we choose R = 20Ω:
- At minimum input: I = 4V / 20Ω = 0.2A ✓
- At maximum input: I = 10V / 20Ω = 0.5A ✓

If we choose R = 5Ω:
- At minimum input: I = 4V / 5Ω = 0.8A ✓
- At maximum input: I = 10V / 5Ω = 2A ✓

**Step 5:** Optimize for load regulation
For better load regulation (ability to handle varying load currents), choose the smaller resistance that allows maximum current swing:

**Answer:** R = 5Ω

This allows the Zener current to vary from 0.8A to 2A as input voltage changes, providing good load regulation capability.

---

## Additional Practice Problems

### Practice Problem 1: Half-Wave Rectifier Analysis

**Given:** Half-wave rectifier with:
- Peak input voltage: 24V
- Load resistance: 1kΩ
- Silicon diode (VF = 0.7V)

**Find:**
(i) Peak output voltage
(ii) Average output voltage
(iii) Peak diode current
(iv) Average diode current

**Solution:**
(i) Peak output voltage = 24V - 0.7V = 23.3V
(ii) Average output voltage = Peak/π = 23.3V/π = 7.42V
(iii) Peak diode current = 23.3V/1kΩ = 23.3mA
(iv) Average diode current = Peak/π = 23.3mA/π = 7.42mA

### Practice Problem 2: Full-Wave Bridge Rectifier

**Given:** Full-wave bridge rectifier with:
- RMS input voltage: 20V
- Load resistance: 500Ω
- Four silicon diodes

**Find:**
(i) Peak output voltage
(ii) Average output voltage
(iii) Ripple factor

**Solution:**
(i) Peak input = 20V × √2 = 28.28V
    Peak output = 28.28V - 2(0.7V) = 26.88V
(ii) Average output = 2 × Peak/π = 2 × 26.88V/π = 17.1V
(iii) Ripple factor = 0.48 (theoretical for full-wave)

### Practice Problem 3: BJT LED Driver

**Given:** NPN BJT LED driver circuit:
- Supply voltage: 5V
- LED forward voltage: 2V
- LED current: 20mA
- BJT β = 100
- Base voltage: 3.3V

**Find:**
(i) Collector resistor value
(ii) Base current
(iii) Base resistor value

**Solution:**
(i) RC = (VCC - VLED)/ILED = (5V - 2V)/20mA = 150Ω
(ii) IB = IC/β = 20mA/100 = 0.2mA
(iii) RB = (VB - VBE)/IB = (3.3V - 0.7V)/0.2mA = 13kΩ

---

## Key Formulas Summary

**Diode Characteristics:**
- Forward voltage drop: VF ≈ 0.7V (Silicon), 0.3V (Germanium)
- Diode equation: I = IS(e^(VD/VT) - 1)

**Rectifier Analysis:**
- Half-wave average: Vavg = Vpeak/π
- Full-wave average: Vavg = 2Vpeak/π
- RMS value: VRMS = Vpeak/√2

**Zener Regulator:**
- Zener voltage: V = VZ + IZRZ
- Series resistance: R = (Vin - VZ)/(IZ + IL)
- Power dissipation: PZ = VZ × IZ

**BJT Relationships:**
- Current gain: β = IC/IB
- Current relationship: IE = IB + IC
- Saturation: VCE(sat) ≈ 0.2V
- Cut-off: IC ≈ 0, IB ≈ 0

**Power Calculations:**
- Power dissipation: P = V × I = I²R = V²/R
- Efficiency: η = Pout/Pin × 100%