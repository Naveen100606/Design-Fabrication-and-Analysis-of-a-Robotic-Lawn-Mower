# Design, Fabrication and Analysis of a Robotic Lawn Mower

**Course:** Design of Machine Elements  
**Semester:** Spring Semester 2025–2026  
**Supervisor:** Dr. Krishna Mohan Kumar

## 1. Introduction

This project focuses on the design, fabrication, and structural analysis of a four-wheel robotic lawn mower intended for grass-cutting applications. The chassis was designed using Autodesk Fusion 360 and fabricated using 3D-printed polylactic acid (PLA). The robot incorporates four DC geared motors for locomotion and a centrally mounted rotary blade for grass cutting.

Analytical calculations and finite element analysis (FEA) using ANSYS were performed to evaluate the structural strength, deformation, fatigue behaviour, and dynamic characteristics of the chassis.

## 2. Objectives

- To design a four-wheel robotic lawn mower chassis using Fusion 360.
- To fabricate the chassis using 3D printing.
- To perform analytical force and stress calculations.
- To evaluate von-Mises stress, deformation, and factor of safety using ANSYS.
- To investigate fatigue life under repeated loading.
- To determine natural frequencies through modal analysis.
- To study the vibration response of the chassis using harmonic response analysis.

## 3. System Design

The robotic lawn mower consists of a chassis, four wheels, DC geared motors, a rotary cutting blade, a blade support structure, a battery, a Raspberry Pi controller, motor drivers, sensors, and mounting brackets.

The chassis was designed to provide structural support for the mechanical and electrical components while maintaining a compact and lightweight configuration. Four driven wheels provide locomotion, with differential wheel speeds used to control the direction of movement.

The cutting mechanism consists of a centrally mounted rotary blade supported by the chassis. The structural design considers the loads associated with the mounted components and the operating conditions of the robot.

## 4. CAD Design and Fabrication

The chassis and mechanical components were modelled using Autodesk Fusion 360. The design was developed to accommodate the motors, wheels, cutting mechanism, controller, and battery.

The chassis was fabricated using PLA through 3D printing. This manufacturing method was selected because it supports rapid prototyping, lightweight structures, and the production of complex geometries.

## 5. Analytical Calculations

Analytical calculations were performed to estimate the forces and stresses acting on the chassis. The loading conditions considered included the weight of the components, wheel reactions, motor loads, and potential vibration forces.

The fundamental equilibrium equations used were:

\[
\sum F_x=0,\qquad \sum F_y=0
\]

\[
\sum M=0
\]

The following relations were considered for stress calculations.

**Normal stress:**

\[
\sigma=\frac{F}{A}
\]

**Bending stress:**

\[
\sigma_b=\frac{Mc}{I}
\]

**Average shear stress:**

\[
\tau=\frac{V}{A}
\]

These calculations provided an analytical basis for evaluating the structural behaviour of the chassis and comparing it with the numerical simulation results.

## 6. ANSYS Finite Element Analysis

ANSYS was used to investigate the structural and dynamic behaviour of the chassis. The analyses included static structural, fatigue, modal, and harmonic response analyses.

### 6.1 Static Structural Analysis

Static structural analysis was performed to determine the stress distribution and deformation under the applied loading and boundary conditions.

The maximum equivalent von-Mises stress was approximately **0.156 MPa**. The maximum stress concentration occurred near the central mounting hole, where the geometric discontinuity influenced the local stress distribution.

The maximum total deformation was approximately **4.37 × 10⁻⁴ mm**. The minimum reported factor of safety was approximately **15**, indicating a substantial safety margin under the simulated conditions.

### 6.2 Fatigue Analysis

Fatigue analysis was conducted to assess the response of the chassis to repeated loading. Potential sources of cyclic loading included wheel movement, blade-induced vibration, and interaction with uneven ground.

The reported minimum fatigue life was approximately **10⁶ cycles**. The analysis also highlighted mounting-hole regions as areas requiring attention because of local stress concentration.

### 6.3 Modal Analysis

Modal analysis was performed to determine the natural frequencies and corresponding vibration modes of the chassis.

The first natural frequency was approximately **319.72 Hz**, while the higher modes reached approximately **1553.7 Hz**.

These results help identify the dynamic characteristics of the structure and assess the possibility of resonance when subjected to periodic excitation.

### 6.4 Harmonic Response Analysis

Harmonic response analysis was performed over a frequency range of **40–400 Hz** to evaluate the response of the chassis to sinusoidal excitation.

The maximum reported displacement was approximately **2.97 × 10⁻⁶ m**. The frequency response showed a peak near the first natural frequency, indicating a potential resonance region within the investigated range.

The results provide information about the vibration response of the chassis under the specified excitation and simulation conditions.

## 7. Summary of Results

| Analysis | Parameter | Reported result |
|---|---|---:|
| Static structural | Maximum von-Mises stress | 0.156 MPa |
| Static structural | Maximum total deformation | 4.37 × 10⁻⁴ mm |
| Static structural | Minimum factor of safety | Approximately 15 |
| Fatigue | Minimum fatigue life | Approximately 10⁶ cycles |
| Modal | First natural frequency | 319.72 Hz |
| Modal | Higher natural frequencies | Up to approximately 1553.7 Hz |
| Harmonic response | Frequency range | 40–400 Hz |
| Harmonic response | Maximum displacement | 2.97 × 10⁻⁶ m |

*Note: These values correspond to the reported simulation results and depend on the material properties, geometry, applied loads, mesh, and boundary conditions.*

## 8. Conclusion

The project involved the design and fabrication of a four-wheel robotic lawn mower chassis using Fusion 360 and 3D printing. Analytical calculations and ANSYS simulations were used to investigate the structural strength and dynamic behaviour of the chassis.

The static structural analysis indicated low deformation and a reported minimum factor of safety of approximately 15 under the specified loading conditions. Fatigue analysis was used to estimate the life under repeated loading, while modal and harmonic response analyses provided information about the natural frequencies and vibration behaviour of the structure.

The analyses identified the central mounting-hole region as an area of stress concentration. Overall, the project provided practical experience in CAD modelling, engineering mechanics, strength of materials, finite element analysis, fatigue assessment, and structural dynamics.

## 9. Software and Tools

- Autodesk Fusion 360 — CAD modelling
- ANSYS — Structural and dynamic analysis
- 3D printing — Chassis fabrication

## 10. References

- ANSYS documentation for static structural, fatigue, modal, and harmonic response analysis.
- Course materials for Design of Machine Elements.
- Project CAD models, analytical calculations, and simulation results.
