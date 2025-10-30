---
title: "Exercise Solutions - Electronics for IoT"
date: "2024-01-01"
thumbnail: "/assets/img/exercise-solutions-bg.jpg"
---

# Exercise Solutions: Chapter 4 - Electronics for IoT

*Complete solutions to all exercises from Chapter 4, with detailed explanations and step-by-step working.*

---

## Part A: Multiple Choice Questions

### 1. Which type of transistor is voltage-controlled?
**Answer: (c) FET**

**Explanation:** Field Effect Transistors (FETs) are controlled by voltage applied to the gate terminal, creating an electric field that modulates the channel conductivity. BJTs are current-controlled devices, while SCRs are triggered by current pulses.

### 2. In an N-channel JFET, the gate is made of:
**Answer: (b) P-type material**

**Explanation:** In N-channel JFETs, the channel is N-type semiconductor, and the gate is formed by P-type material. This creates a P-N junction that is reverse-biased during normal operation to control the depletion region width.

### 3. The input impedance of a MOSFET is:
**Answer: (c) Very high (>10^12 Ω)**

**Explanation:** MOSFETs have an insulated gate structure with silicon dioxide between the gate and channel. This provides virtually infinite input resistance, typically greater than 10^12 ohms, making them ideal for high-impedance applications.

### 4. MOSFET stands for:
**Answer: (b) Metal-Oxide-Semiconductor Field Effect Transistor**

**Explanation:** MOSFET is the acronym for Metal-Oxide-Semiconductor Field Effect Transistor, referring to its construction with a metal gate, oxide insulation layer, and semiconductor channel.

### 5. A thyristor has how many layers?
**Answer: (c) Four**

**Explanation:** Thyristors have a four-layer P-N-P-N structure, creating three P-N junctions. This unique structure enables the latching behavior characteristic of thyristors.

### 6. The SCR remains ON until:
**Answer: (b) Current drops below holding current**

**Explanation:** Once triggered, an SCR remains in the conducting state until the forward current drops below the holding current value. This latching behavior is fundamental to SCR operation.

### 7. A UJT has:
**Answer: (a) One junction**

**Explanation:** Despite having three terminals, a UJT (Unijunction Transistor) has only one P-N junction between the emitter and the base bar, hence the name "unijunction."

### 8. The intrinsic standoff ratio of a UJT is typically:
**Answer: (b) 0.5 to 0.8**

**Explanation:** The intrinsic standoff ratio (η) of a UJT typically ranges from 0.5 to 0.8, determining the voltage at which the device triggers. This parameter is crucial for oscillator design.

### 9. Enhancement mode MOSFETs are:
**Answer: (a) Normally OFF**

**Explanation:** Enhancement mode MOSFETs have no conducting channel without gate voltage applied, making them normally OFF devices. A gate voltage above the threshold is required to create the channel.

### 10. Which device is best for high-frequency switching?
**Answer: (c) MOSFET**

**Explanation:** MOSFETs have the fastest switching speeds due to their voltage-controlled operation and lack of minority carrier storage. This makes them ideal for high-frequency applications like switching power supplies.

---

## Part B: Short Answer Questions

### 1. What is the main difference between a JFET and a MOSFET?

**Answer:**
The main difference lies in the gate construction and control mechanism:

**JFET (Junction FET):**
- Gate is a reverse-biased P-N junction
- Direct electrical connection to semiconductor
- Lower input impedance (though still high)
- Only depletion mode operation

**MOSFET (Metal-Oxide-Semiconductor FET):**
- Gate is insulated by oxide layer (SiO₂)
- No direct electrical connection to channel
- Extremely high input impedance
- Both enhancement and depletion modes available

This fundamental difference makes MOSFETs more versatile and suitable for integrated circuits.

### 2. Explain the pinch-off condition in a JFET.

**Answer:**
Pinch-off occurs when the gate voltage becomes sufficiently negative (for N-channel JFET) that the depletion regions from both sides of the channel meet, effectively closing the conducting path.

**Mechanism:**
1. Gate-source voltage increases reverse bias
2. Depletion region widens into the channel
3. Channel becomes progressively narrower
4. At pinch-off voltage (VP), channel is completely depleted
5. Drain current approaches zero

**Mathematical relationship:**
When VGS = VP, ID ≈ 0 (except for small leakage current)

This condition defines the boundary between normal operation and cut-off.

### 3. What are the three terminals of a thyristor and their functions?

**Answer:**
The three terminals of a thyristor (SCR) are:

**1. Anode (A):**
- Positive terminal for main current flow
- Connected to P-layer in P-N-P-N structure
- Current enters through this terminal when conducting

**2. Cathode (K):**
- Negative terminal for main current flow  
- Connected to N-layer in P-N-P-N structure
- Current exits through this terminal when conducting

**3. Gate (G):**
- Control terminal for triggering
- Small positive current pulse initiates conduction
- Connected to P-layer adjacent to cathode
- No control over turn-off (latching device)

### 4. Define threshold voltage in MOSFETs.

**Answer:**
Threshold voltage (VTH) is the minimum gate-to-source voltage required to create a conducting channel in an enhancement mode MOSFET.

**Key characteristics:**
- **N-channel**: Positive threshold (typically 1-4V)
- **P-channel**: Negative threshold (typically -1 to -4V)
- **Temperature dependent**: Decreases with increasing temperature
- **Manufacturing parameter**: Varies between devices

**Significance:**
- Below VTH: MOSFET is OFF (no channel)
- Above VTH: MOSFET begins conducting
- Critical for logic level compatibility
- Determines switching voltage levels

### 5. How does a UJT differ from a conventional transistor?

**Answer:**
UJTs differ significantly from conventional transistors (BJTs) in structure and operation:

**Structure:**
- **UJT**: Single P-N junction, three terminals (E, B1, B2)
- **BJT**: Two P-N junctions, three terminals (E, B, C)

**Operation:**
- **UJT**: Exhibits negative resistance characteristics
- **BJT**: Exhibits positive current gain

**Applications:**
- **UJT**: Primarily oscillators and timing circuits
- **BJT**: Amplification and switching

**Control mechanism:**
- **UJT**: Voltage-controlled with switching action
- **BJT**: Current-controlled with amplification

**Current flow:**
- **UJT**: Unidirectional with specific trigger point
- **BJT**: Bidirectional with linear control

---

## Part C: Long Answer Questions

### 1. Explain the construction and working principle of an N-channel JFET with neat diagrams.

**Answer:**

#### Construction of N-channel JFET

**Physical Structure:**
An N-channel JFET consists of:
- **N-type semiconductor bar**: Forms the main current-carrying channel
- **P-type gate regions**: Diffused into both sides of the N-channel
- **Ohmic contacts**: Source and drain connected to channel ends
- **Gate contact**: Connected to P-type regions

```
     Source (S)
         |
    ┌────┴────┐
    │ N-type  │  ← P-type Gate (G)
    │ Channel │
    │         │  ← P-type Gate (G)  
    └────┬────┘
         |
      Drain (D)
```

#### Working Principle

**1. Basic Operation:**
- Current flows through N-channel from source to drain
- Gate-channel junction is reverse-biased
- Depletion region controls channel width

**2. Effect of Gate Voltage:**

**Zero Gate Voltage (VGS = 0):**
- Small depletion region exists due to built-in potential
- Maximum channel width available
- Maximum drain current flows (IDSS)

**Negative Gate Voltage (VGS < 0):**
- Reverse bias increases depletion region width
- Channel becomes narrower
- Drain current decreases

**Pinch-off Voltage (VGS = VP):**
- Depletion regions meet, blocking the channel
- Drain current approaches zero
- Device is in cut-off state

**3. Current-Voltage Relationships:**

**Transfer Characteristic:**
ID = IDSS × (1 - VGS/VP)²

**Output Characteristic:**
Shows three regions:
- **Ohmic region**: Linear relationship between VDS and ID
- **Saturation region**: Constant current with varying VDS
- **Breakdown region**: Excessive voltage causes damage

#### Characteristics and Parameters

**Key specifications:**
- **IDSS**: 2-20 mA (typical)
- **VP**: -2 to -10V (typical)
- **gm**: 1000-5000 μS
- **Input resistance**: >10^8 Ω

### 2. Compare enhancement and depletion mode MOSFETs.

**Answer:**

#### Enhancement Mode MOSFETs

**Characteristics:**
- **Normally OFF device**: No channel exists without gate voltage
- **Channel creation**: Gate voltage creates inversion layer
- **Threshold voltage**: Must exceed VTH for conduction
- **Most common type**: Used in digital and analog circuits

**N-Channel Enhancement:**
- **Gate voltage**: Positive (>VTH) to create electron channel
- **Operation**: VGS > VTH creates conducting channel
- **Applications**: Logic circuits, power switching

**P-Channel Enhancement:**
- **Gate voltage**: Negative (<VTH) to create hole channel  
- **Operation**: VGS < VTH creates conducting channel
- **Applications**: Complementary circuits (CMOS)

#### Depletion Mode MOSFETs

**Characteristics:**
- **Normally ON device**: Channel exists without gate voltage
- **Channel modulation**: Gate voltage modifies existing channel
- **Bidirectional control**: Can enhance or deplete channel
- **Less common**: Specialized applications

**N-Channel Depletion:**
- **Zero gate voltage**: Maximum channel conductivity
- **Positive gate**: Enhances channel (more current)
- **Negative gate**: Depletes channel (less current)
- **Applications**: Constant current sources, analog switches

#### Detailed Comparison

| Parameter | Enhancement Mode | Depletion Mode |
|-----------|------------------|----------------|
| **Default State** | OFF (no channel) | ON (channel present) |
| **Gate Voltage Required** | Above threshold | Any voltage |
| **Channel Formation** | Induced by gate field | Pre-existing |
| **Control Range** | Unidirectional enhancement | Bidirectional control |
| **Power Consumption** | Lower (OFF when unused) | Higher (always conducting) |
| **Applications** | Digital switching, logic | Analog circuits, current sources |
| **Circuit Complexity** | Simple (single supply) | More complex (dual supply) |
| **Manufacturing** | Standard process | Additional implant steps |

#### Circuit Symbols and Operation

**Enhancement Mode Symbols:**
- **N-channel**: Broken line in channel (normally open)
- **P-channel**: Broken line with arrow pointing in

**Depletion Mode Symbols:**
- **N-channel**: Solid line in channel (normally closed)
- **P-channel**: Solid line with arrow pointing in

#### Operating Equations

**Enhancement Mode:**
- **Cut-off**: ID = 0 when VGS < VTH
- **Linear**: ID = K[(VGS-VTH)VDS - VDS²/2] when VDS < VGS-VTH
- **Saturation**: ID = K(VGS-VTH)² when VDS ≥ VGS-VTH

**Depletion Mode:**
- **All regions**: ID = IDSS[1 - VGS/VP]² for VGS ≤ VP
- **Enhancement**: ID > IDSS when VGS > 0

### 3. Describe the operation of a Silicon Controlled Rectifier (SCR) and its applications.

**Answer:**

#### SCR Construction and Structure

**Four-Layer Configuration:**
The SCR consists of alternating P-N-P-N layers creating a unique switching device:

```
Anode (A) → P₁ layer
           N₁ layer  ← Gate (G)
           P₂ layer
Cathode(K)→ N₂ layer
```

**Three P-N Junctions:**
- **J₁**: P₁-N₁ junction (anode-gate region)
- **J₂**: N₁-P₂ junction (middle junction)  
- **J₃**: P₂-N₂ junction (gate-cathode region)

#### Two-Transistor Model

**Equivalent Circuit:**
The SCR can be modeled as two interconnected transistors:
- **PNP transistor**: P₁-N₁-P₂ structure
- **NPN transistor**: N₁-P₂-N₂ structure
- **Positive feedback**: Collector of each drives base of the other

**Regenerative Action:**
1. Initial trigger starts small current in one transistor
2. This current drives the base of the second transistor  
3. Second transistor output reinforces first transistor
4. Process continues until both saturate (latch ON)

#### SCR Operation Modes

**1. Forward Blocking State:**
- **Conditions**: Anode positive, no gate current
- **Junction bias**: J₁ forward, J₂ reverse, J₃ forward
- **Behavior**: J₂ blocks current, device acts like open switch
- **Current**: Small leakage current only

**2. Forward Conduction State:**
- **Conditions**: Triggered by gate current or breakover voltage
- **Junction bias**: All junctions forward-biased
- **Behavior**: Low resistance path, acts like closed switch
- **Current**: Limited only by external circuit

**3. Reverse Blocking State:**
- **Conditions**: Cathode positive relative to anode
- **Junction bias**: J₁ reverse, J₂ forward, J₃ reverse
- **Behavior**: Blocks reverse current like a diode
- **Current**: Small reverse leakage

#### Triggering Methods

**1. Gate Triggering (Normal Method):**
- Small positive current pulse to gate
- Reduces breakover voltage significantly
- Controlled turn-on timing
- Most common method

**2. Voltage Triggering:**
- Forward voltage exceeds breakover voltage
- Avalanche breakdown in blocking junction
- Uncontrolled method (usually avoided)

**3. Light Triggering (LASCR):**
- Light photons create electron-hole pairs
- Provides electrical isolation
- Used in high-voltage applications

**4. Temperature Triggering:**
- High temperature reduces breakover voltage
- Usually unwanted triggering method
- Requires thermal management

#### SCR Characteristics and Parameters

**Key Ratings:**
- **VDRM**: Peak repetitive forward voltage (200-6000V typical)
- **VRRM**: Peak repetitive reverse voltage  
- **IT(AV)**: Average forward current (1A-3000A typical)
- **ITSM**: Peak surge current capability
- **IGT**: Gate trigger current (0.1-200 mA typical)
- **VGT**: Gate trigger voltage (0.7-3V typical)
- **IH**: Holding current (5-200 mA typical)

**Protection Requirements:**
- **dv/dt protection**: RC snubber circuits prevent false triggering
- **di/dt protection**: Series inductance limits current rise rate
- **Thermal protection**: Adequate heat sinking and temperature monitoring

#### SCR Applications

**1. AC Power Control:**
- **Phase control circuits**: Variable power to resistive loads
- **Motor speed control**: AC motor drives
- **Light dimmers**: Incandescent lamp control
- **Heating control**: Electric furnaces and heaters

**2. DC Power Applications:**
- **Battery chargers**: Controlled charging current
- **DC motor drives**: Speed and torque control  
- **Switching regulators**: Power supply circuits
- **Inverters**: DC to AC conversion

**3. Protection Circuits:**
- **Crowbar protection**: Overvoltage protection for power supplies
- **Circuit breakers**: Electronic overcurrent protection
- **Surge suppressors**: Transient voltage protection
- **Arc fault detectors**: Electrical safety systems

**4. IoT and Modern Applications:**
- **Smart home devices**: Controllable power outlets
- **Industrial automation**: Motor control and process heating
- **Renewable energy**: Solar inverter protection
- **Electric vehicles**: Battery management and charging

#### Advantages and Limitations

**Advantages:**
- High current and voltage capability
- Low power loss when conducting
- Fast switching (microsecond range)
- Electrical isolation (gate circuit)
- High reliability and long life

**Limitations:**
- Cannot be turned off by gate control
- Requires external commutation for turn-off
- Sensitive to dv/dt and di/dt
- Gate power required for triggering
- Limited to unidirectional current flow

### 4. Explain the characteristics and applications of UJT in relaxation oscillators.

**Answer:**

#### UJT Construction and Basic Operation

**Physical Structure:**
- **N-type silicon bar**: Forms the main conductive path
- **P-type emitter**: Injected into the middle of the bar
- **Two base contacts**: B₁ and B₂ at opposite ends
- **Ohmic contacts**: Low resistance connections

**Internal Resistance Distribution:**
The silicon bar acts as a voltage divider:
- **RB1**: Resistance from emitter to B₁
- **RB2**: Resistance from emitter to B₂  
- **Total resistance**: RBB = RB1 + RB2 (typically 5-10 kΩ)

#### UJT Characteristics

**Intrinsic Standoff Ratio (η):**
η = RB1/(RB1 + RB2) = RB1/RBB

**Typical values**: 0.5 to 0.8
**Significance**: Determines trigger voltage level

**Emitter Characteristic Curve:**
The UJT exhibits a unique voltage-current relationship with three distinct regions:

**1. Cut-off Region:**
- **Condition**: VE < VP (peak voltage)
- **Behavior**: High resistance, minimal current
- **Emitter junction**: Reverse-biased
- **Applications**: Energy storage phase

**2. Negative Resistance Region:**
- **Condition**: VP > VE > VV (valley voltage)
- **Behavior**: Current increases while voltage decreases
- **Unique property**: Negative resistance characteristic
- **Applications**: Switching and oscillation

**3. Saturation Region:**
- **Condition**: VE > VV, IE > IV
- **Behavior**: Low resistance, linear operation
- **Emitter junction**: Forward-biased
- **Applications**: Pulse generation

#### Key UJT Parameters

**Peak Voltage (VP):**
VP = ηVBB + VD

Where:
- η = intrinsic standoff ratio
- VBB = voltage between B₁ and B₂
- VD = diode forward voltage drop (≈0.7V)

**Other Critical Parameters:**
- **Peak current (IP)**: Minimum current to maintain conduction
- **Valley voltage (VV)**: Minimum operating voltage  
- **Valley current (IV)**: Current at valley point
- **Interbase resistance (RBB)**: Total resistance between bases

#### UJT Relaxation Oscillator

**Basic Circuit Configuration:**
```
     +VCC
       |
       R (Charging resistor)
       |
    C  |  UJT
    ═══┼──E
       |   |
       |   B₂──── +VCC
       |   |
       └───B₁──── Output
           |
          R₁ (Load resistor)
           |
          GND
```

**Operating Principle:**

**1. Charging Phase:**
- Capacitor C charges through resistor R
- UJT is in cut-off state (high resistance)
- VE increases exponentially toward VCC
- Duration determined by RC time constant

**2. Triggering Phase:**
- When VE reaches VP, UJT triggers
- Emitter resistance drops dramatically
- Capacitor discharges rapidly through emitter-B₁ path
- Sharp current pulse appears at B₁

**3. Recovery Phase:**
- Capacitor voltage drops below VV
- UJT returns to cut-off state
- Charging cycle begins again
- Process repeats periodically

#### Oscillator Frequency Calculation

**Approximate Frequency:**
f ≈ 1/(RC ln(1/(1-η)))

**More Precise Formula:**
f = 1/(RC ln((VCC-VV)/(VCC-VP)))

**Design Considerations:**
- **R value**: Must allow sufficient charging current
- **C value**: Determines timing and frequency
- **VCC level**: Affects frequency and amplitude
- **Load resistance**: Influences output pulse shape

#### Frequency Stability Factors

**Temperature Effects:**
- η decreases slightly with temperature
- VD increases with temperature  
- Net effect: Frequency increases with temperature
- Compensation techniques may be required

**Supply Voltage Variation:**
- Frequency relatively independent of VCC
- Good regulation over wide voltage range
- Inherent advantage of UJT oscillators

**Component Tolerances:**
- R and C tolerances directly affect frequency
- Precision components improve stability
- Trimming resistors allow fine adjustment

#### UJT Applications

**1. Timing Circuits:**
- **Delay generators**: Precise timing delays
- **Pulse generators**: Sharp timing pulses
- **Clock sources**: Low-frequency clock generation
- **Time base circuits**: Reference timing for other circuits

**2. Trigger Circuits:**
- **SCR triggering**: Phase control applications
- **Triac firing**: AC power control
- **Flash units**: Camera flash timing
- **Ignition systems**: Automotive applications

**3. Voltage Sensing:**
- **Over/under voltage detection**: Protection circuits
- **Battery monitoring**: Charge level indication
- **Threshold detection**: Level sensing applications
- **Alarm circuits**: Security and monitoring systems

**4. Modern IoT Applications:**
- **Sensor timing**: Periodic sensor readings
- **Watchdog timers**: System monitoring
- **Sleep/wake cycles**: Power management
- **Communication timing**: Protocol timing generation

#### Advantages of UJT Oscillators

**1. Simplicity:**
- Few external components required
- Easy to design and implement
- Low cost solution

**2. Reliability:**
- Inherently stable operation
- Wide temperature range
- Long service life

**3. Performance:**
- Good frequency stability
- Sharp output pulses
- Wide frequency range (Hz to kHz)

**4. Flexibility:**
- Easy frequency adjustment
- Multiple output options
- Scalable design

#### Limitations and Considerations

**1. Frequency Range:**
- Limited to relatively low frequencies
- Not suitable for high-frequency applications
- Maximum frequency limited by device characteristics

**2. Output Characteristics:**
- Pulse output only (not sinusoidal)
- Limited output power
- May require buffering for heavy loads

**3. Modern Alternatives:**
- Microcontroller timers often preferred
- IC oscillators offer better performance
- Digital solutions provide more flexibility

**4. Design Constraints:**
- Careful component selection required
- PCB layout considerations for stability
- Temperature compensation may be needed

---

## Part D: Numerical Problems

### 1. A JFET has IDSS = 12 mA and VP = -4V. Calculate the drain current when VGS = -1.5V.

**Given:**
- IDSS = 12 mA
- VP = -4V  
- VGS = -1.5V

**Formula:**
ID = IDSS × (1 - VGS/VP)²

**Solution:**
ID = 12 × (1 - (-1.5)/(-4))²
ID = 12 × (1 - 1.5/4)²
ID = 12 × (1 - 0.375)²
ID = 12 × (0.625)²
ID = 12 × 0.390625
ID = 4.69 mA

**Answer: ID = 4.69 mA**

### 2. An N-channel MOSFET has VTH = 2V and K = 0.5 mA/V². Find ID when VGS = 5V in saturation region.

**Given:**
- VTH = 2V
- K = 0.5 mA/V²
- VGS = 5V
- Operating in saturation region

**Formula for saturation region:**
ID = K × (VGS - VTH)²

**Solution:**
ID = 0.5 × (5 - 2)²
ID = 0.5 × (3)²
ID = 0.5 × 9
ID = 4.5 mA

**Answer: ID = 4.5 mA**

### 3. A UJT has η = 0.6 and is connected with VBB = 12V. Calculate the peak voltage VP if VD = 0.7V.

**Given:**
- η = 0.6
- VBB = 12V
- VD = 0.7V

**Formula:**
VP = η × VBB + VD

**Solution:**
VP = 0.6 × 12 + 0.7
VP = 7.2 + 0.7
VP = 7.9V

**Answer: VP = 7.9V**

### 4. Calculate the transconductance of a JFET if a change in VGS from -1V to -1.5V causes ID to change from 8 mA to 6 mA.

**Given:**
- VGS1 = -1V, ID1 = 8 mA
- VGS2 = -1.5V, ID2 = 6 mA

**Formula:**
gm = ΔID/ΔVGS

**Solution:**
ΔVGS = VGS2 - VGS1 = -1.5 - (-1) = -0.5V
ΔID = ID2 - ID1 = 6 - 8 = -2 mA

gm = |-2 mA|/|-0.5V| = 2 mA/0.5V = 4 mS

**Answer: gm = 4 mS (millisiemens)**

### 5. For a UJT relaxation oscillator with R = 47 kΩ, C = 0.1 μF, and η = 0.7, calculate the oscillation frequency.

**Given:**
- R = 47 kΩ = 47 × 10³ Ω
- C = 0.1 μF = 0.1 × 10⁻⁶ F
- η = 0.7

**Formula:**
f = 1/(RC × ln(1/(1-η)))

**Solution:**
RC = 47 × 10³ × 0.1 × 10⁻⁶ = 4.7 × 10⁻³ s

ln(1/(1-η)) = ln(1/(1-0.7)) = ln(1/0.3) = ln(3.333) = 1.204

f = 1/(4.7 × 10⁻³ × 1.204)
f = 1/(5.659 × 10⁻³)
f = 176.7 Hz

**Answer: f ≈ 177 Hz**

---

## Additional Practice Problems

### Problem 6: MOSFET Power Calculation
A power MOSFET operates with VDS = 10V and ID = 2A. If RDS(on) = 0.1Ω, calculate the power dissipated in the ON state.

**Solution:**
P = ID² × RDS(on) = (2)² × 0.1 = 4 × 0.1 = 0.4W

### Problem 7: SCR Holding Current
An SCR has a holding current of 15 mA. If the load resistance is 50Ω and supply voltage is 12V, determine if the SCR will remain ON after triggering.

**Solution:**
Load current = V/R = 12V/50Ω = 0.24A = 240 mA
Since 240 mA > 15 mA (holding current), the SCR will remain ON.

### Problem 8: JFET Voltage Divider Bias
A JFET with IDSS = 10 mA and VP = -3V is biased with RG = 1MΩ and RS = 300Ω. Calculate the operating point when VDD = 15V.

**Solution:**
This requires iterative solution:
VGS = -ID × RS
ID = IDSS(1 - VGS/VP)²

Substituting and solving iteratively:
ID ≈ 3.2 mA, VGS ≈ -0.96V

---

*These exercise solutions provide comprehensive coverage of FET, thyristor, and UJT calculations commonly encountered in IoT electronics applications. Practice with similar problems to strengthen your understanding of these important semiconductor devices.*