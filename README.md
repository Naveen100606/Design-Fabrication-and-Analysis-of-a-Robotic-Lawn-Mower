# Design-Fabrication-and-Analysis-of-a-Robotic-Lawn-Mower
Designed a 3D-printed four-wheel robotic lawn mower chassis using Fusion 360 and performed analytical stress calculations and ANSYS FEA. Evaluated von-Mises stress, deformation, factor of safety, fatigue life, modal frequencies, and harmonic response to assess structural integrity and dynamic stability.
# 🤖 Design, Fabrication and Analysis of a Robotic Lawn Mower

## 📌 Project Overview

This project focuses on the **mechanical design, structural analysis, and dynamic evaluation of a four-wheel robotic lawn mower** developed for grass-cutting applications on a predefined path.

The robot uses a compact wheeled locomotion system powered by **DC geared motors**, with a centrally mounted rotary cutting blade. The chassis was designed in **Fusion 360** and manufactured using **3D-printed PLA**.

The mechanical structure was evaluated using analytical calculations and **ANSYS finite element analysis (FEA)** to study structural strength, deformation, fatigue behaviour, natural frequencies, and harmonic response.

---

## 🎯 Objectives

* Design a structurally safe robotic lawn mower chassis.
* Develop a compact four-wheel locomotion mechanism.
* Design the chassis and mechanical components using CAD.
* Manufacture the chassis using 3D printing.
* Perform analytical stress and force calculations.
* Evaluate structural behaviour using ANSYS FEA.
* Study stress concentration around mounting interfaces.
* Determine the factor of safety under operating loads.
* Evaluate fatigue behaviour under repeated loading.
* Determine natural frequencies using modal analysis.
* Study vibration behaviour using harmonic response analysis.

---

## ⚙️ System Design

The robotic lawn mower consists of the following major subsystems:

* Main chassis
* Four-wheel drive system
* DC geared motors
* Rotary cutting blade
* Blade support structure
* Raspberry Pi controller
* Motor drivers
* Battery system
* Sensor interfaces
* L-brackets and mounting components

The design uses **conventional wheels instead of tracked locomotion**, reducing mechanical complexity while providing maneuverability and efficient movement.

---

## 🛞 Locomotion Mechanism

The robot uses independently driven wheels with differential speed control.

| Wheel Control            | Result              |
| ------------------------ | ------------------- |
| Equal wheel speed        | Straight motion     |
| Higher left-wheel speed  | Right turn          |
| Higher right-wheel speed | Left turn           |
| Opposite wheel rotation  | Zero-radius turning |

Four DC motors are connected to the wheels to provide the required motion and steering capability.

---

## 🔪 Cutting Mechanism

A centrally mounted rotary cutting blade is used for grass cutting.

The blade rotates at high speed and is supported by the mechanical structure of the chassis. The resulting operational forces and vibration loads were considered during the structural analysis.

---

## 🧩 Chassis Design

The chassis was designed using **Fusion 360** and manufactured using **3D-printed PLA**.

PLA was selected for the chassis because of its:

* Lightweight nature
* Ease of manufacturing
* Suitability for rapid prototyping
* Ease of producing complex geometries

The chassis supports the motors, wheels, cutting mechanism, controller, battery, and other components.

---

## 📐 Force Analysis

The chassis experiences multiple loading conditions during operation, including:

* Chassis weight
* Motor reaction forces
* Ground reaction forces
* Blade vibration forces
* Wheel friction forces

Free-body diagrams and equilibrium equations were used to determine reactions and internal loading.

The fundamental equilibrium conditions considered were:

```text
ΣFx = 0

ΣFy = 0

ΣM = 0
```

---

## 🧮 Analytical Stress Analysis

Several types of stresses were considered during the mechanical analysis:

* Normal stress
* Bending stress
* Shear stress
* Torsional stress
* Principal stress
* Equivalent von-Mises stress

Basic relations used include:

### Normal Stress

```text
σ = F / A
```

### Bending Stress

```text
σb = Mc / I
```

### Shear Stress

```text
τ = V / A
```

The calculated stresses were subsequently used to evaluate the structural safety of the components.

---

# 💻 ANSYS FEA

Finite Element Analysis was performed using **ANSYS** to evaluate the mechanical and dynamic behaviour of the lawn mower chassis.

The analyses included:

* Static Structural Analysis
* Equivalent von-Mises Stress Analysis
* Total Deformation Analysis
* Factor of Safety Analysis
* Fatigue Analysis
* Modal Analysis
* Harmonic Response Analysis

---

## 🔩 Static Structural Analysis

### Equivalent von-Mises Stress

The static structural analysis was used to determine the stress distribution throughout the chassis.

The maximum equivalent stress obtained from the ANSYS analysis was approximately:

```text
Maximum von-Mises Stress ≈ 0.156 MPa
```

The highest stress concentration occurred near the **central mounting hole**, where the geometric discontinuity caused localized stress concentration.

The overall stress distribution indicated adequate load transfer through the chassis.

---

## 📏 Total Deformation

The total deformation analysis identified the maximum deformation near the central mounting-hole region.

The maximum deformation obtained was approximately:

```text
Maximum Deformation ≈ 4.37 × 10⁻⁴ mm
```

The small deformation indicates that the chassis maintains adequate stiffness under the applied loading conditions.

---

## 🛡️ Factor of Safety

The ANSYS factor-of-safety analysis produced a minimum factor of safety of approximately:

```text
Minimum FOS ≈ 15
```

This indicates that the evaluated chassis configuration remains within the specified loading limits under the simulated conditions.

---

# 🔄 Fatigue Analysis

Fatigue analysis was performed to evaluate the behaviour of the chassis under repeated and fluctuating loads.

Potential cyclic loading sources include:

* Wheel movement
* Blade rotation
* Structural vibration
* Uneven ground interaction
* Repeated operational loading

The analysis examined equivalent alternating stress and fatigue life.

The report indicates a minimum fatigue life on the order of:

```text
≈ 10⁶ cycles
```

with the highest alternating stresses concentrated around geometric discontinuities and mounting-hole regions.

---

# 📳 Modal Analysis

Modal analysis was performed using **ANSYS Modal** to determine the natural frequencies of the chassis.

The first natural frequency obtained was approximately:

```text
First Natural Frequency ≈ 319.72 Hz
```

Higher modes were observed at progressively increasing frequencies, with frequencies reaching approximately:

```text
≈ 1553.7 Hz
```

The modal analysis was used to understand the dynamic characteristics of the chassis and identify potential resonance regions.

---

# 📈 Harmonic Response Analysis

Harmonic response analysis was performed to study the response of the chassis to sinusoidal excitation.

### Frequency Range

```text
40 Hz – 400 Hz
```

The displacement response showed a peak near the first natural frequency.

The maximum displacement was approximately:

```text
≈ 2.97 × 10⁻⁶ m
```

The force response also showed a peak near the same frequency region, indicating resonance behaviour around the first natural frequency.

The phase response exhibited a rapid phase shift around the resonance region, which is characteristic of a dynamically excited mechanical structure.

---

# 🔍 Stress Concentration

A significant focus of the analysis was the effect of **geometric discontinuities** on stress distribution.

The central mounting-hole region showed localized stress concentration in the static, fatigue, and dynamic analyses.

This demonstrates the importance of considering:

* Hole geometry
* Mounting interfaces
* Edge transitions
* Load transfer paths
* Geometric discontinuities

during mechanical design.

---

# 📊 Analysis Summary

| Analysis          | Main Parameter           | Approximate Result |
| ----------------- | ------------------------ | -----------------: |
| Static Structural | Maximum von-Mises stress |          0.156 MPa |
| Static Structural | Maximum deformation      |     4.37 × 10⁻⁴ mm |
| Static Structural | Minimum FOS              |               ≈ 15 |
| Fatigue           | Minimum life             |       ≈ 10⁶ cycles |
| Modal             | First natural frequency  |          319.72 Hz |
| Modal             | Higher modes             |  Up to ≈ 1553.7 Hz |
| Harmonic          | Frequency range          |          40–400 Hz |
| Harmonic          | Maximum displacement     |    ≈ 2.97 × 10⁻⁶ m |

> **Note:** Values are based on the simulation results reported in the project report and correspond to the specific material properties, geometry, loading conditions, and boundary conditions used in the analysis.

---

# 🛠️ Software & Tools

### CAD

* Autodesk Fusion 360

### FEA

* ANSYS
* Static Structural
* Fatigue Analysis
* Modal Analysis
* Harmonic Response

### Manufacturing

* 3D Printing
* PLA-based prototyping

### Mechanical Engineering

* Engineering Mechanics
* Strength of Materials
* Stress Analysis
* Fatigue
* Vibrations
* Machine Design

---

# 📁 Suggested Repository Structure

```text
Robotic-Lawn-Mower/
│
├── README.md
│
├── CAD/
│   ├── Chassis/
│   ├── Wheel_Assembly/
│   └── Blade_Mount/
│
├── ANSYS/
│   ├── Static_Structural/
│   ├── Fatigue/
│   ├── Modal/
│   └── Harmonic_Response/
│
├── Calculations/
│   ├── Force_Analysis/
│   ├── Stress_Calculations/
│   └── Fatigue_Calculations/
│
├── Images/
│   ├── CAD/
│   ├── Prototype/
│   ├── Stress_Analysis/
│   ├── Deformation/
│   ├── Fatigue/
│   ├── Modal/
│   └── Harmonic_Response/
│
├── Documentation/
│   └── Project_Report.pdf
│
└── Results/
    └── Simulation_Results/
```

---

# 📷 Project Images

Add your actual project images here:

### CAD Model

```text
/images/CAD/chassis.png
```

### ANSYS Stress Analysis

```text
/images/Stress_Analysis/von_mises.png
```

### Deformation

```text
/images/Deformation/total_deformation.png
```

### Modal Analysis

```text
/images/Modal/first_mode.png
```

### Harmonic Response

```text
/images/Harmonic_Response/frequency_response.png
```

---

# 📌 Key Engineering Takeaways

This project provided practical experience in:

* Mechanical system design
* CAD modelling
* Load and force analysis
* Strength of materials
* Stress concentration
* Finite Element Analysis
* Fatigue analysis
* Structural dynamics
* Modal analysis
* Harmonic response
* Mechanical prototyping
* Design validation

The project demonstrates the application of **analytical mechanical calculations together with numerical FEA** to evaluate the structural and dynamic performance of a mechanical system.

---


### Supervisor

**Dr. Krishna Mohan Kumar**

---

## 🎓 Course

**Design of Machine Elements**
Spring Semester 2025–2026
