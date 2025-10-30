---
title: "Exercise Solutions - Electric Circuits"
date: "2024-01-01"
thumbnail: "/assets/img/exercise-solutions-bg.jpg"
---

# Exercise Solutions: Chapter 2 - Electric Circuits

*Note: These solutions are provided for practice and understanding. They demonstrate proper application of circuit analysis techniques.*

## Multiple Choice Questions

### Question 1: In a series circuit, which quantity remains the same throughout all components?
**Answer: c. Current**

**Explanation:** In series circuits, there is only one path for current to flow, so the same current must pass through each component. Voltage divides among components based on their resistance values, but current remains constant throughout the series path.

### Question 2: In a parallel circuit, which quantity remains the same across all branches?
**Answer: a. Voltage**

**Explanation:** In parallel circuits, all components are connected between the same two points, so they all experience the same potential difference (voltage). Current divides among the branches based on their resistance values.

### Question 3: Kirchhoff's Voltage Law states that:
**Answer: b. The sum of voltage drops around any closed loop equals the applied voltage**

**Explanation:** KVL is based on conservation of energy. As you trace around any closed loop, the energy supplied by voltage sources must equal the energy consumed by resistive elements. Mathematically, the algebraic sum of all voltages around a loop equals zero.

### Question 4: Kirchhoff's Current Law applies to:
**Answer: c. Nodes or junctions in a circuit**

**Explanation:** KCL states that the algebraic sum of currents entering and leaving any node equals zero. This is based on conservation of charge - current flowing into a junction must equal current flowing out.

### Question 5: The total resistance of three 12Ω resistors connected in parallel is:
**Answer: a. 4Ω**

**Explanation:** For parallel resistors: 1/R_total = 1/R₁ + 1/R₂ + 1/R₃ = 1/12 + 1/12 + 1/12 = 3/12 = 1/4. Therefore, R_total = 4Ω.

---

## Short Answer Questions

### Question 1: What are the four essential components of any electric circuit?

**Answer:** 
1. **Conducting Wire:** Provides the path for electric current to flow throughout the circuit
2. **Voltage Source:** Supplies the electrical energy that drives current through the circuit (batteries, power supplies, generators)
3. **Load:** Consumes electrical energy and converts it to other forms of energy (light bulbs, motors, resistors)
4. **Control Device:** Allows operation control of the circuit (switches, relays, variable resistors)

### Question 2: Explain the difference between open and closed circuits.

**Answer:**
**Closed Circuit:** A complete, unbroken path exists for current to flow from the positive terminal of the voltage source, through all components, and back to the negative terminal. Current flows and the circuit operates normally.

**Open Circuit:** The current path is broken at some point, preventing current flow. This can occur due to an open switch, broken wire, or disconnected component. No current flows and the circuit does not operate.

### Question 3: What is a node in an electric circuit?

**Answer:** A node is a junction point in an electric circuit where two or more circuit elements connect together. At a node, conductors from different branches meet, allowing current to divide or combine. Nodes are essential reference points for applying Kirchhoff's Current Law during circuit analysis.

### Question 4: State Kirchhoff's Voltage Law and explain its physical significance.

**Answer:** 
**Statement:** The algebraic sum of all voltages around any closed loop in a circuit equals zero.

**Physical Significance:** KVL is based on the conservation of energy principle. As electric current travels around a closed path, the total energy gained from voltage sources must equal the total energy lost in resistive components. This means voltage rises (sources) must balance voltage drops (loads) around any loop.

### Question 5: State Kirchhoff's Current Law and explain its physical significance.

**Answer:**
**Statement:** The algebraic sum of all currents entering and leaving any node in a circuit equals zero.

**Physical Significance:** KCL is based on the conservation of electric charge. Electric charge cannot accumulate at a point in a circuit under steady-state conditions. Therefore, the total current flowing into a junction must equal the total current flowing out of that junction.

---

## Detailed Answer Questions

### Question 1: Compare and contrast series and parallel circuit connections in detail.

**Answer:**

**Series Circuits:**

**Connection Method:** Components are connected end-to-end, forming a single continuous path for current flow.

**Current Characteristics:** The same current flows through all components because there is only one path available. If current changes anywhere, it changes everywhere simultaneously.

**Voltage Characteristics:** The total applied voltage divides among the components. Each component receives a portion of the total voltage based on its resistance value relative to the total circuit resistance.

**Resistance Calculation:** Total resistance equals the sum of individual resistances: R_total = R₁ + R₂ + R₃ + ...

**Advantages:**
- Simple circuit design and construction
- Uses fewer connecting wires
- Single switch can control entire circuit
- Lower cost for basic applications

**Disadvantages:**
- If one component fails, entire circuit stops working
- Components cannot be controlled independently
- Different components may receive suboptimal voltage levels
- Adding more components reduces current to all components

**Parallel Circuits:**

**Connection Method:** Components are connected across common points, providing multiple independent paths for current flow.

**Current Characteristics:** Total current divides among the branches. Each branch carries current based on its resistance value, with lower resistance branches carrying more current.

**Voltage Characteristics:** All components receive the same voltage, equal to the applied source voltage.

**Resistance Calculation:** Total resistance is calculated using: 1/R_total = 1/R₁ + 1/R₂ + 1/R₃ + ...

**Advantages:**
- Components operate independently
- Each component receives full source voltage
- Circuit remains functional if one component fails
- Components can be controlled individually
- Adding more components does not affect existing component operation

**Disadvantages:**
- More complex wiring required
- Higher total current consumption
- More expensive installation costs
- Requires more sophisticated control systems

**Practical Applications:**
- **Series:** Christmas lights (some types), flashlights, simple doorbells
- **Parallel:** Household outlets, car lighting systems, computer components

### Question 2: Explain Kirchhoff's laws with practical examples and mathematical applications.

**Answer:**

**Kirchhoff's Voltage Law (KVL):**

**Theoretical Foundation:** Based on conservation of energy, KVL states that the algebraic sum of voltage rises and drops around any closed loop equals zero.

**Mathematical Expression:** ΣV = 0 around any closed loop

**Sign Convention:**
- Voltage rises (across sources): Positive when traversing from negative to positive terminal
- Voltage drops (across resistors): Negative when traversing in direction of current flow

**Practical Example 1 - Simple Series Circuit:**
Consider a circuit with 24V battery and three resistors (4Ω, 6Ω, 2Ω) in series.

**Solution:**
1. Total resistance: R_total = 4 + 6 + 2 = 12Ω
2. Circuit current: I = V/R = 24V/12Ω = 2A
3. Voltage drops: V₁ = 2A × 4Ω = 8V, V₂ = 2A × 6Ω = 12V, V₃ = 2A × 2Ω = 4V
4. KVL verification: +24V - 8V - 12V - 4V = 0 ✓

**Kirchhoff's Current Law (KCL):**

**Theoretical Foundation:** Based on conservation of charge, KCL states that the algebraic sum of currents entering and leaving any node equals zero.

**Mathematical Expression:** ΣI = 0 at any node

**Sign Convention:**
- Currents entering node: Positive
- Currents leaving node: Negative

**Practical Example 2 - Parallel Circuit Analysis:**
Consider a node where 6A enters and splits into three branches with resistances 3Ω, 6Ω, and 2Ω, all connected to 12V.

**Solution:**
1. Branch currents: I₁ = 12V/3Ω = 4A, I₂ = 12V/6Ω = 2A, I₃ = 12V/2Ω = 6A
2. KCL at entering node: 6A - 4A - 2A - 6A = -6A (incorrect)
3. Recalculation needed: Total current should be I₁ + I₂ + I₃ = 4A + 2A + 6A = 12A
4. KCL verification: +12A - 4A - 2A - 6A = 0 ✓

**Complex Circuit Application:**
For circuits with multiple loops and nodes, systematic application involves:
1. Identify all independent loops and nodes
2. Write KVL equations for each independent loop
3. Write KCL equations for each independent node
4. Solve the resulting system of simultaneous equations
5. Verify solutions by checking power balance

### Question 3: Describe different types of circuit components and their functions in electric circuits.

**Answer:**

**Resistors:**

**Function:** Resistors oppose current flow and control current levels in circuits.

**Types and Applications:**
- **Fixed Resistors:** Constant resistance value, used for current limiting, voltage division, and circuit protection
- **Variable Resistors (Potentiometers):** Adjustable resistance, used for volume controls, dimmer switches, and calibration
- **Thermistors:** Temperature-dependent resistance, used in temperature sensors and compensation circuits

**Circuit Behavior:**
- Follow Ohm's law: V = IR
- Dissipate power as heat: P = I²R
- Can be connected in series or parallel combinations

**Capacitors:**

**Function:** Store electrical energy in an electric field between two conducting plates.

**Key Properties:**
- Block DC current while allowing AC current
- Store and release electrical charge
- Provide timing functions in circuits
- Filter unwanted frequency components

**Types and Applications:**
- **Electrolytic Capacitors:** High capacitance values, used in power supplies for smoothing voltage
- **Ceramic Capacitors:** Stable performance, used in high-frequency circuits
- **Film Capacitors:** Low leakage, used in precision timing circuits

**Circuit Behavior:**
- Charging: Current high initially, decreases exponentially
- Discharging: Voltage high initially, decreases exponentially
- Energy storage: E = ½CV²

**Inductors:**

**Function:** Store electrical energy in a magnetic field created by current flow through a coil.

**Key Properties:**
- Oppose changes in current flow
- Allow DC current while opposing AC current changes
- Create magnetic fields for motor operation
- Provide filtering in power circuits

**Types and Applications:**
- **Air Core Inductors:** Linear response, used in radio frequency circuits
- **Iron Core Inductors:** High inductance, used in power applications
- **Ferrite Core Inductors:** High frequency performance, used in switching circuits

**Circuit Behavior:**
- Voltage proportional to rate of current change: V = L(di/dt)
- Energy storage: E = ½LI²
- Impedance increases with frequency in AC circuits

**Switches:**

**Function:** Provide manual or automatic control of current flow.

**Types:**
- **Manual Switches:** SPST (Single Pole Single Throw), DPDT (Double Pole Double Throw)
- **Automatic Switches:** Relays, contactors, circuit breakers
- **Semiconductor Switches:** Transistors, thyristors, MOSFETs

**Applications:**
- Circuit protection (circuit breakers)
- Remote control (relays)
- Signal switching (transistors)
- Power control (contactors)

### Question 4: Explain the process of analyzing complex circuits using Kirchhoff's laws.

**Answer:**

**Systematic Circuit Analysis Procedure:**

**Step 1: Circuit Preparation**
- Draw the circuit clearly with all components labeled
- Assign reference directions for all unknown currents
- Mark all node points clearly
- Identify all independent loops

**Step 2: Choose Analysis Method**
- **Node Voltage Method:** Best when circuit has fewer nodes than loops
- **Mesh Current Method:** Best when circuit has fewer loops than nodes
- **Combined Method:** Use both for complex circuits

**Step 3: Apply Kirchhoff's Laws**

**For Node Voltage Method:**
1. Select reference node (usually ground)
2. Assign voltage variables to remaining nodes
3. Apply KCL at each independent node
4. Express currents in terms of node voltages using Ohm's law
5. Solve resulting system of equations

**For Mesh Current Method:**
1. Identify independent loops (meshes)
2. Assign mesh current variables (usually clockwise)
3. Apply KVL around each mesh
4. Express voltages in terms of mesh currents using Ohm's law
5. Solve resulting system of equations

**Step 4: Mathematical Solution**
- Set up matrix equations for systematic solution
- Use substitution, elimination, or matrix methods
- Solve for unknown currents and voltages

**Step 5: Verification**
- Check all solutions using original circuit equations
- Verify power balance: Total power supplied = Total power consumed
- Confirm all KCL and KVL equations are satisfied

**Practical Example - Complex Circuit Analysis:**

**Given Circuit:** Two voltage sources (12V and 8V) with three resistors (4Ω, 6Ω, 3Ω) in a network configuration.

**Mesh Analysis Solution:**
1. **Identify Meshes:** Two independent loops
2. **Mesh Equations:**
   - Mesh 1: 12V = I₁(4Ω) + (I₁-I₂)(6Ω)
   - Mesh 2: -8V = (I₂-I₁)(6Ω) + I₂(3Ω)
3. **Simplify:**
   - 12 = 10I₁ - 6I₂
   - -8 = -6I₁ + 9I₂
4. **Solve System:**
   - From equation 1: I₁ = (12 + 6I₂)/10
   - Substitute into equation 2: -8 = -6((12 + 6I₂)/10) + 9I₂
   - Solve for I₂, then find I₁
5. **Calculate Branch Currents and Voltages**

**Applications in Real Systems:**
- Power distribution network analysis
- Electronic circuit design verification
- Fault location in electrical systems
- Optimization of circuit performance

---

## Problem Solutions

### Problem 1: Series Circuit Analysis

**Given:**
- Three resistors in series: R₁ = 5Ω, R₂ = 10Ω, R₃ = 15Ω
- Applied voltage: V = 30V

**Find:** Current through circuit and voltage across each resistor

**Solution:**
**Step 1:** Calculate total resistance
R_total = R₁ + R₂ + R₃ = 5Ω + 10Ω + 15Ω = 30Ω

**Step 2:** Calculate circuit current
I = V_total / R_total = 30V / 30Ω = 1A

**Step 3:** Calculate voltage across each resistor
- V₁ = I × R₁ = 1A × 5Ω = 5V
- V₂ = I × R₂ = 1A × 10Ω = 10V
- V₃ = I × R₃ = 1A × 15Ω = 15V

**Step 4:** Verify using KVL
V_total = V₁ + V₂ + V₃ = 5V + 10V + 15V = 30V ✓

**Answer:** Circuit current = 1A, Voltages: V₁ = 5V, V₂ = 10V, V₃ = 15V

### Problem 2: Parallel Circuit Analysis

**Given:**
- Three resistors in parallel: R₁ = 6Ω, R₂ = 3Ω, R₃ = 2Ω
- Applied voltage: V = 12V

**Find:** Total current and current through each resistor

**Solution:**
**Step 1:** Calculate individual branch currents
- I₁ = V / R₁ = 12V / 6Ω = 2A
- I₂ = V / R₂ = 12V / 3Ω = 4A
- I₃ = V / R₃ = 12V / 2Ω = 6A

**Step 2:** Calculate total current using KCL
I_total = I₁ + I₂ + I₃ = 2A + 4A + 6A = 12A

**Step 3:** Verify using total resistance method
1/R_total = 1/R₁ + 1/R₂ + 1/R₃ = 1/6 + 1/3 + 1/2 = 1/6 + 2/6 + 3/6 = 6/6 = 1
R_total = 1Ω
I_total = V / R_total = 12V / 1Ω = 12A ✓

**Answer:** Total current = 12A, Branch currents: I₁ = 2A, I₂ = 4A, I₃ = 6A

### Problem 3: Kirchhoff's Laws Application

**Given:**
- Circuit with two loops and three resistors
- V₁ = 20V, V₂ = 10V, R₁ = 4Ω, R₂ = 6Ω, R₃ = 2Ω

**Find:** All branch currents using mesh analysis

**Solution:**
**Step 1:** Define mesh currents I_a and I_b (clockwise)

**Step 2:** Write mesh equations using KVL
- Mesh A: 20V = I_a(4Ω) + (I_a - I_b)(2Ω)
- Mesh B: -10V = (I_b - I_a)(2Ω) + I_b(6Ω)

**Step 3:** Simplify equations
- Equation 1: 20 = 4I_a + 2I_a - 2I_b = 6I_a - 2I_b
- Equation 2: -10 = 2I_b - 2I_a + 6I_b = -2I_a + 8I_b

**Step 4:** Solve system of equations
From equation 1: I_a = (20 + 2I_b)/6
Substitute into equation 2: -10 = -2((20 + 2I_b)/6) + 8I_b
-10 = -(40 + 4I_b)/6 + 8I_b
-60 = -40 - 4I_b + 48I_b
-20 = 44I_b
I_b = -20/44 = -5/11 A ≈ -0.45A

I_a = (20 + 2(-5/11))/6 = (20 - 10/11)/6 = (220/11 - 10/11)/6 = (210/11)/6 = 35/11 A ≈ 3.18A

**Step 5:** Calculate branch currents
- Current through R₁: I₁ = I_a = 35/11 A
- Current through R₂: I₂ = I_b = -5/11 A (flows opposite to assumed direction)
- Current through R₃: I₃ = I_a - I_b = 35/11 - (-5/11) = 40/11 A ≈ 3.64A

**Answer:** I₁ = 3.18A, I₂ = 0.45A (opposite direction), I₃ = 3.64A

### Problem 4: Power Calculation in Circuits

**Given:**
- Series-parallel combination circuit
- Total voltage: 24V
- R₁ = 8Ω (series), R₂ = 6Ω and R₃ = 12Ω (parallel branch)

**Find:** Total power consumed and power in each resistor

**Solution:**
**Step 1:** Calculate equivalent resistance of parallel branch
1/R_parallel = 1/R₂ + 1/R₃ = 1/6 + 1/12 = 2/12 + 1/12 = 3/12 = 1/4
R_parallel = 4Ω

**Step 2:** Calculate total circuit resistance
R_total = R₁ + R_parallel = 8Ω + 4Ω = 12Ω

**Step 3:** Calculate total current
I_total = V_total / R_total = 24V / 12Ω = 2A

**Step 4:** Calculate voltage across parallel branch
V_parallel = I_total × R_parallel = 2A × 4Ω = 8V

**Step 5:** Calculate individual currents and powers
- Current through R₁: I₁ = I_total = 2A
- Power in R₁: P₁ = I₁² × R₁ = (2A)² × 8Ω = 32W

- Current through R₂: I₂ = V_parallel / R₂ = 8V / 6Ω = 4/3 A
- Power in R₂: P₂ = I₂² × R₂ = (4/3)² × 6Ω = 32/3 W ≈ 10.67W

- Current through R₃: I₃ = V_parallel / R₃ = 8V / 12Ω = 2/3 A
- Power in R₃: P₃ = I₃² × R₃ = (2/3)² × 12Ω = 16/3 W ≈ 5.33W

**Step 6:** Calculate total power
P_total = P₁ + P₂ + P₃ = 32W + 32/3W + 16/3W = 32W + 48/3W = 32W + 16W = 48W

**Verification:** P_total = V_total × I_total = 24V × 2A = 48W ✓

**Answer:** Total power = 48W, Individual powers: P₁ = 32W, P₂ = 10.67W, P₃ = 5.33W

---

## Additional Practice Problems

### Extra Problem 1: Complex Network Analysis

**Given:** Bridge circuit with five resistors and one voltage source
**Objective:** Determine if bridge is balanced and calculate all currents

### Extra Problem 2: Capacitive Circuit Analysis

**Given:** RC circuit with charging capacitor
**Objective:** Calculate time constants and energy storage

### Extra Problem 3: Mixed AC/DC Circuit

**Given:** Circuit with both AC and DC sources
**Objective:** Apply superposition principle for analysis

---

## Key Formulas Summary

**Series Circuits:**
- Total Resistance: R_total = R₁ + R₂ + R₃ + ...
- Current: Same throughout (I₁ = I₂ = I₃ = I_total)
- Voltage: V_total = V₁ + V₂ + V₃ + ...

**Parallel Circuits:**
- Total Resistance: 1/R_total = 1/R₁ + 1/R₂ + 1/R₃ + ...
- Voltage: Same across all (V₁ = V₂ = V₃ = V_total)
- Current: I_total = I₁ + I₂ + I₃ + ...

**Kirchhoff's Laws:**
- KVL: ΣV = 0 (around any closed loop)
- KCL: ΣI = 0 (at any node)

**Power Formulas:**
- P = VI (general power formula)
- P = I²R (power in terms of current and resistance)
- P = V²/R (power in terms of voltage and resistance)

**Energy Formulas:**
- E = Pt (electrical energy)
- E = ½CV² (capacitor energy storage)
- E = ½LI² (inductor energy storage)