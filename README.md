# 🔎 Metal Detector Using NE555 Timer IC

An affordable electronics project demonstrating a metal detector circuit built using the NE555 timer IC, an inductive coil, and basic electronic components.

<p align="center">
  <img src="circuit/circuit-diagram.png" alt="NE555 Timer IC Metal Detector Circuit Diagram" width="750">
</p>

## 📌 Project Overview

The **Metal Detector Using NE555 Timer IC** is an electronics project developed as part of the PCB Design and Fabrication subject during the second year of Electronics and Telecommunication Engineering.

The prototype uses an NE555 timer IC, an inductive coil, resistors, capacitors, a red LED, and a buzzer. It is powered by a 9V battery and assembled on a perforated PCB.

The project explores the practical application of timer circuits, inductive sensing, PCB design, soldering, and hardware testing.

## 🎯 Project Objectives

* Understand the operation of the NE555 timer IC.
* Design and assemble a metal detector circuit.
* Explore inductive sensing and electromagnetic interactions with nearby metal.
* Learn PCB layout, component placement, and soldering.
* Use a red LED and buzzer as output indicators.
* Test the prototype using different metallic objects.
* Develop practical analog electronics and hardware debugging skills.

## 🧰 Hardware Components

The following components are documented in the project report.

| No. | Component                   | Specification                | Purpose                                |
| --: | --------------------------- | ---------------------------- | -------------------------------------- |
|   1 | NE555 timer IC              | DIP-8 package                | Timer and oscillator circuit           |
|   2 | Resistor                    | 1 kΩ                         | Current limiting and circuit operation |
|   3 | Resistors                   | 10 kΩ, 2 units               | Timing network                         |
|   4 | Capacitors                  | 2.2 µF, 2 units              | Timing network                         |
|   5 | Capacitor                   | 100 nF                       | Noise bypassing                        |
|   6 | Inductor coil               | 10 mH, as documented         | Metal-sensing element                  |
|   7 | Red LED                     | 5 mm                         | Visual indication                      |
|   8 | Buzzer                      | Active buzzer, as documented | Audible indication                     |
|   9 | Battery                     | 9V                           | Power supply                           |
|  10 | ON/OFF switch               | SPST                         | Power control                          |
|  11 | IC socket                   | 8-pin                        | Removable mounting for the NE555       |
|  12 | PCB                         | Approximately 2 × 3 inches   | Component mounting                     |
|  13 | Battery connector and wires | Suitable for the circuit     | Electrical connections                 |

*Note: Component specifications are taken from the project report. Verify the final assembled circuit and component values before reproducing the design.*

## ⚙️ Working Principle

### 1. Power Supply

A 9V battery supplies power to the circuit. An ON/OFF switch controls the power supply.

### 2. NE555 Timer IC

The NE555 timer is the primary active component. The project report describes it as operating in astable mode to generate a continuously repeating output signal.

The timing behaviour depends on the connected resistors, capacitors, and the actual circuit topology.

### 3. Detection Coil

The circuit includes an inductive coil intended to sense nearby metallic objects.

When metal approaches a coil carrying a varying current, electromagnetic interactions can alter the coil's effective electrical behaviour. Whether this produces a measurable change in the detector's output depends on the circuit design.

### 4. Output Indication

The circuit includes two output indicators:

* **Red LED:** Provides a visual indication.
* **Buzzer:** Provides an audible indication.

The project report describes changes in the output response when metal approaches the coil.

The exact relationship between the coil, oscillator, and output indicators should be verified against the final circuit and experimental measurements.

## 🔌 Circuit Diagram

The following diagram documents the proposed circuit arrangement for the NE555 timer-based metal detector.

![NE555 Timer IC Metal Detector Circuit Diagram](circuit/circuit-diagram.png)

The circuit diagram identifies the power supply, NE555 timer IC, resistors, capacitors, inductive coil, LED, buzzer, and ON/OFF switch.

**Important:** Refer to the diagram and verify component connections before assembling or modifying the circuit.

## 🖥️ PCB Design

PCB design was part of the project, including component placement and track routing.

### PCB Track Layout

The track layout illustrates the intended electrical connections between the circuit components.

![PCB Track Layout](images/metal%20detector%202.jpeg)

### PCB Component Layout

The component layout illustrates the planned placement of the components on the PCB.

![PCB Component Layout](images/metal%20detector%201.jpeg)

### Soldering and Wiring

The soldering-side photograph documents the physical assembly and wiring of the prototype.

![PCB Soldering Side](images/metal%20detector%203.jpeg)

## 📸 Working Prototype

The completed prototype consists of the detection coil, NE555-based circuit, red LED, ON/OFF switch, and 9V battery.

![Metal Detector Prototype](images/metal%20detector.jpeg)

The photograph documents the physical implementation of the project.

## 🧪 Testing and Reported Results

The project report describes testing with several objects, including a coin, a metal spoon, an iron bolt, aluminium foil, and a plastic object.

The following table reproduces the reported observations.

| Test object    | Material reported                  | Reported detection distance |
| -------------- | ---------------------------------- | --------------------------: |
| 1 Rupee coin   | Steel, as identified in the report |                      4–5 cm |
| Metal spoon    | Stainless steel                    |                      7–8 cm |
| Iron bolt      | Ferrous iron                       |                     8–10 cm |
| Aluminium foil | Aluminium                          |                      2–3 cm |
| Plastic pen    | Plastic                            |                No detection |

**These are results reported in the project document, not independently verified measurements.** Actual performance can vary with the object, coil geometry, circuit construction, and test conditions.

The report also describes an estimated normal oscillation frequency of approximately 31 Hz. This value should be checked against the actual circuit and measured output waveform before being treated as a verified operating frequency.

## 🧠 Engineering Concepts Demonstrated

This project provides practical exposure to:

* NE555 timer IC operation.
* Oscillator circuits.
* Resistor-capacitor timing networks.
* Inductors and electromagnetic interactions.
* Basic electronic circuit design.
* PCB layout and component placement.
* Through-hole soldering.
* Power supply connections.
* Hardware testing and troubleshooting.
* Technical documentation.

## ⚠️ Limitations

* The prototype's detection range is limited and depends on the test object.
* Detection performance may vary with coil geometry and orientation.
* The device does not identify the exact type of metal.
* The reported detection distances require repeatable experimental verification.
* The relationship between the coil and oscillator response needs confirmation from the actual circuit.
* No independently verified false-alarm rate or long-term reliability data is available in this repository.
* The device is an educational prototype, not a certified security or industrial inspection instrument.

## 🚀 Future Improvements

Potential improvements include:

* Verify the circuit connections against the final PCB.
* Measure the output waveform using an oscilloscope.
* Compare oscillator behaviour with and without nearby metal.
* Conduct repeatable detection-range tests using different objects.
* Record test conditions and measured results.
* Improve PCB routing and soldering documentation.
* Add a detailed component-to-pin connection table.
* Improve mechanical protection and portability.

## 🔋 Power and Safety

The documented prototype uses a 9V battery.

Before powering or modifying the circuit:

* Verify the battery polarity.
* Check the NE555 pin orientation.
* Inspect solder joints for shorts.
* Confirm the polarity of electrolytic capacitors and the LED.
* Verify the buzzer's voltage and current requirements.
* Disconnect the battery before soldering or changing connections.

## 📂 Repository Structure

```text
N555-Timer-IC-Based-Metal-Detector/
│
├── README.md
│
├── circuit/
│   ├── circuit-diagram.png
│   └── README.md
│
└── images/
    ├── README.md
    ├── metal detector.jpeg
    ├── metal detector 1.jpeg
    ├── metal detector 2.jpeg
    └── metal detector 3.jpeg
```

This structure documents the circuit, PCB layouts, and physical prototype.

## 👨‍🎓 Project Information

* **Project title:** Design and Implementation of a Metal Detector Using NE555 Timer IC
* **Department:** Electronics and Telecommunication Engineering
* **Institution:** D. Y. Patil College of Engineering, Akurdi, Pune
* **Academic year:** 2025–2026
* **Subject:** PCB Design and Fabrication
* **Project type:** Academic electronics hardware project

## 🤝 Acknowledgements

This project was completed as part of an academic group project under the guidance of the subject instructor.

## 📜 Disclaimer

This project is intended for educational purposes. Its reported detection range and behaviour should not be assumed to represent guaranteed performance. Verify the circuit and test results before using the design in practical applications.
