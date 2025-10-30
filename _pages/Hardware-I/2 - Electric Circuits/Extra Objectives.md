---
title: "Extra Objectives - Electric Circuits"
date: "2024-01-01"
thumbnail: "/assets/img/extra-objectives-bg.jpg"
---

# Extra Objectives: Chapter 2 - Electric Circuits

*Note: These fill-in-the-blank questions are for interactive learning and exam preparation. Click on the hidden words to reveal answers and explanations.*

<style>
.blank {
    background-color: #f0f0f0;
    border: 2px dashed #ccc;
    padding: 2px 8px;
    cursor: pointer;
    border-radius: 4px;
    display: inline-block;
    min-width: 60px;
    text-align: center;
}

.blank:hover {
    background-color: #e0e0e0;
}

.revealed {
    background-color: #d4edda;
    border: 2px solid #c3e6cb;
    color: #155724;
}

.explanation {
    background-color: #f8f9fa;
    border-left: 4px solid #007bff;
    padding: 10px;
    margin: 10px 0;
    display: none;
    border-radius: 4px;
}

.explanation.show {
    display: block;
}
</style>

<script>
function revealAnswer(element, answer, explanationId) {
    element.innerHTML = answer;
    element.classList.add('revealed');
    element.style.cursor = 'default';
    
    const explanation = document.getElementById(explanationId);
    if (explanation) {
        explanation.classList.add('show');
    }
}
</script>

## Fill-in-the-Blank Questions

### Question 1
An electric circuit must have a <span class="blank" onclick="revealAnswer(this, 'closed path', 'exp1')">____</span> for current to flow from the positive terminal through components and back to the negative terminal.

<div id="exp1" class="explanation">
<strong>Explanation:</strong> A complete, unbroken path is essential for current flow. If there is any break in the circuit (open switch, broken wire, or disconnected component), current cannot flow and the circuit becomes non-functional.
</div>

### Question 2
In a series circuit, the <span class="blank" onclick="revealAnswer(this, 'current', 'exp2')">____</span> remains the same through all components, while voltage divides among them.

<div id="exp2" class="explanation">
<strong>Explanation:</strong> Series circuits have only one path for current flow, so the same current must pass through each component. However, each component drops a portion of the total voltage based on its resistance value.
</div>

### Question 3
In a parallel circuit, the <span class="blank" onclick="revealAnswer(this, 'voltage', 'exp3')">____</span> across all branches is the same, while current divides among the branches.

<div id="exp3" class="explanation">
<strong>Explanation:</strong> Parallel circuits connect all components between the same two points, ensuring each component experiences the full source voltage. Current divides based on each branch's resistance value.
</div>

### Question 4
Kirchhoff's Voltage Law states that the algebraic sum of all voltages around any <span class="blank" onclick="revealAnswer(this, 'closed loop', 'exp4')">____</span> equals zero.

<div id="exp4" class="explanation">
<strong>Explanation:</strong> KVL is based on conservation of energy. When you traverse any closed path and return to the starting point, the net energy change must be zero, so voltage rises must equal voltage drops.
</div>

### Question 5
Kirchhoff's Current Law applies to <span class="blank" onclick="revealAnswer(this, 'nodes', 'exp5')">____</span> and states that the sum of currents entering equals the sum of currents leaving.

<div id="exp5" class="explanation">
<strong>Explanation:</strong> KCL is based on conservation of charge. At any junction point (node), charge cannot accumulate, so all current flowing in must equal all current flowing out.
</div>

### Question 6
A <span class="blank" onclick="revealAnswer(this, 'node', 'exp6')">____</span> is a junction point where two or more circuit elements connect together.

<div id="exp6" class="explanation">
<strong>Explanation:</strong> Nodes are essential reference points in circuit analysis. They represent points where currents can divide or combine, making them ideal locations for applying Kirchhoff's Current Law.
</div>

### Question 7
The total resistance of resistors in series is found by <span class="blank" onclick="revealAnswer(this, 'adding', 'exp7')">____</span> all individual resistance values.

<div id="exp7" class="explanation">
<strong>Explanation:</strong> In series circuits, current must pass through each resistor sequentially, so resistances add up: R_total = R₁ + R₂ + R₃ + ... This increases the total opposition to current flow.
</div>

### Question 8
For resistors in parallel, the total resistance is always <span class="blank" onclick="revealAnswer(this, 'less than', 'exp8')">____</span> the smallest individual resistance value.

<div id="exp8" class="explanation">
<strong>Explanation:</strong> Parallel connections provide multiple paths for current flow, reducing total resistance. The formula 1/R_total = 1/R₁ + 1/R₂ + ... always yields a result smaller than any individual resistance.
</div>

### Question 9
<span class="blank" onclick="revealAnswer(this, 'Capacitors', 'exp9')">____</span> store electrical energy in an electric field between two conducting plates.

<div id="exp9" class="explanation">
<strong>Explanation:</strong> Capacitors accumulate electrical charge on their plates when voltage is applied, creating an electric field in the dielectric material between plates. This stored energy can be released when needed.
</div>

### Question 10
<span class="blank" onclick="revealAnswer(this, 'Inductors', 'exp10')">____</span> store electrical energy in a magnetic field created by current flowing through a coil.

<div id="exp10" class="explanation">
<strong>Explanation:</strong> When current flows through an inductor's coil, it creates a magnetic field that stores energy. This energy storage enables applications like transformers, motors, and power supply filtering.
</div>

### Question 11
In DC circuits, capacitors act as <span class="blank" onclick="revealAnswer(this, 'open circuits', 'exp11')">____</span> after they are fully charged.

<div id="exp11" class="explanation">
<strong>Explanation:</strong> Once a capacitor is fully charged to the applied voltage, no more current can flow through it in DC circuits. The capacitor blocks further DC current flow while maintaining its stored charge.
</div>

### Question 12
A <span class="blank" onclick="revealAnswer(this, 'branch', 'exp12')">____</span> is any single circuit element connected between two nodes.

<div id="exp12" class="explanation">
<strong>Explanation:</strong> Branches represent individual circuit elements like resistors, voltage sources, or current sources. Each branch carries a specific current that contributes to the overall circuit behavior.
</div>

### Question 13
When applying KVL, voltage <span class="blank" onclick="revealAnswer(this, 'rises', 'exp13')">____</span> across sources are considered positive, while voltage drops across resistors are negative.

<div id="exp13" class="explanation">
<strong>Explanation:</strong> This sign convention helps maintain consistency when writing KVL equations. Voltage sources provide energy (positive), while resistors consume energy (negative), and the algebraic sum must equal zero.
</div>

### Question 14
The reference direction for current is <span class="blank" onclick="revealAnswer(this, 'arbitrary', 'exp14')">____</span> and does not need to match the actual current direction.

<div id="exp14" class="explanation">
<strong>Explanation:</strong> Reference directions are chosen for mathematical convenience. If the calculated current is positive, it flows in the assumed direction; if negative, it flows in the opposite direction.
</div>

### Question 15
<span class="blank" onclick="revealAnswer(this, 'Mesh analysis', 'exp15')">____</span> uses fictitious loop currents and applies KVL to independent loops.

<div id="exp15" class="explanation">
<strong>Explanation:</strong> Mesh analysis assigns imaginary currents flowing around each independent loop (mesh). These mesh currents automatically satisfy KCL at every node, simplifying the analysis process.
</div>

### Question 16
<span class="blank" onclick="revealAnswer(this, 'Nodal analysis', 'exp16')">____</span> uses node voltages and applies KCL at independent nodes.

<div id="exp16" class="explanation">
<strong>Explanation:</strong> Nodal analysis assigns voltage variables to each independent node (referenced to ground). KCL equations are written at each node with currents expressed in terms of node voltages.
</div>

### Question 17
In household wiring, appliances are connected in <span class="blank" onclick="revealAnswer(this, 'parallel', 'exp17')">____</span> so each receives full voltage and operates independently.

<div id="exp17" class="explanation">
<strong>Explanation:</strong> Parallel wiring ensures each appliance gets the full line voltage (120V or 240V) and can be controlled independently. If one appliance fails, others continue operating normally.
</div>

### Question 18
The <span class="blank" onclick="revealAnswer(this, 'load', 'exp18')">____</span> in a circuit consumes electrical energy and converts it to other forms like light, heat, or motion.

<div id="exp18" class="explanation">
<strong>Explanation:</strong> Loads are the useful components in circuits that perform the desired work. Examples include light bulbs (electrical to light), motors (electrical to mechanical), and speakers (electrical to sound).
</div>

### Question 19
A circuit with a break in the current path is called an <span class="blank" onclick="revealAnswer(this, 'open circuit', 'exp19')">____</span> and no current can flow.

<div id="exp19" class="explanation">
<strong>Explanation:</strong> Open circuits have incomplete paths that prevent current flow. This can result from open switches, broken wires, or disconnected components, making the circuit non-functional.
</div>

### Question 20
<span class="blank" onclick="revealAnswer(this, 'Power', 'exp20')">____</span> in electrical circuits is calculated using P = VI, P = I²R, or P = V²/R.

<div id="exp20" class="explanation">
<strong>Explanation:</strong> These three power formulas are derived from the fundamental relationship P = VI combined with Ohm's law. Choose the appropriate formula based on which quantities are known in the circuit.
</div>

### Question 21
Current division in parallel circuits follows the principle that branches with <span class="blank" onclick="revealAnswer(this, 'lower resistance', 'exp21')">____</span> carry more current.

<div id="exp21" class="explanation">
<strong>Explanation:</strong> In parallel circuits, current divides inversely proportional to resistance. Lower resistance branches offer easier paths for current flow, so they carry larger portions of the total current.
</div>

### Question 22
Voltage division in series circuits means components with <span class="blank" onclick="revealAnswer(this, 'higher resistance', 'exp22')">____</span> drop more voltage.

<div id="exp22" class="explanation">
<strong>Explanation:</strong> In series circuits, voltage divides proportionally to resistance values. Components with higher resistance oppose current flow more, requiring larger voltage drops to drive the same current.
</div>

### Question 23
The <span class="blank" onclick="revealAnswer(this, 'superposition principle', 'exp23')">____</span> allows analysis of circuits with multiple sources by considering one source at a time.

<div id="exp23" class="explanation">
<strong>Explanation:</strong> Superposition works because circuit equations are linear. Analyze the circuit with each independent source active (others set to zero), then sum the individual responses to get the total response.
</div>

### Question 24
<span class="blank" onclick="revealAnswer(this, 'Conservation of energy', 'exp24')">____</span> is the physical principle behind Kirchhoff's Voltage Law.

<div id="exp24" class="explanation">
<strong>Explanation:</strong> Energy cannot be created or destroyed in electrical circuits. KVL ensures that energy supplied by sources equals energy consumed by loads, maintaining energy balance around any closed loop.
</div>

### Question 25
<span class="blank" onclick="revealAnswer(this, 'Conservation of charge', 'exp25')">____</span> is the physical principle behind Kirchhoff's Current Law.

<div id="exp25" class="explanation">
<strong>Explanation:</strong> Electric charge cannot accumulate at a point in steady-state circuits. KCL ensures that charge flowing into any node equals charge flowing out, maintaining charge balance at every junction.
</div>

---

## Interactive Learning Tips

- **Click on each blank** to reveal the answer and read the explanation
- **Review explanations carefully** as they provide additional context beyond basic answers
- **Practice multiple times** to reinforce understanding of circuit analysis concepts
- **Focus on the reasoning** behind each answer to build analytical thinking skills
- **Connect concepts** between different questions to see how circuit principles relate

---

## Additional Practice

After completing all fill-in-the-blanks, try to:

1. **Draw circuit diagrams** for each concept mentioned
2. **Explain each principle** in your own words without looking at explanations
3. **Solve numerical problems** applying these concepts
4. **Create your own examples** of series and parallel circuits
5. **Practice applying Kirchhoff's laws** to simple circuit problems

*Note: These interactive questions reinforce fundamental circuit analysis concepts and prepare you for more advanced electrical engineering topics.*