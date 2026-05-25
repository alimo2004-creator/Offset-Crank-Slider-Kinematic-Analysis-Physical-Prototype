# Offset Crank-Slider: Kinematic Analysis & Physical Prototype

![SolidWorks](https://img.shields.io/badge/SolidWorks-CAD-blue)
![Math](https://img.shields.io/badge/Analysis-Kinematics-success)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

## 📌 Project Overview
This repository contains the mathematical models, CAD files, and documentation for a miniature 5-link physical model of an **offset crank-slider mechanism**. 

The primary objective of this project was to analyze the kinematic motion profiles (position, velocity, and acceleration) across a full 360-degree rotational cycle, identify and correct a theoretical textbook error regarding offset geometry, and empirically validate the mathematical constraints using a fabricated physical prototype.

## 🚀 Key Features & Accomplishments
* **Mathematical Correction:** Identified and resolved a documented textbook error regarding the kinematic equation for offset geometry, resulting in a highly accurate displacement model.
* **Kinematic Simulation:** Calculated peak velocity and acceleration profiles to evaluate the dynamic forces acting on the mechanism links.
* **CAD Modeling:** Designed a precise 5-link structural assembly in SolidWorks to ensure strict geometric alignment and constraint validation.
* **Physical Prototyping:** Fabricated and assembled the miniature physical model to bridge the gap between theoretical calculations and real-world mechanical motion.

## 📐 Mathematical Modeling
In a standard in-line crank-slider, the slider axis intersects the crank pivot. In this **offset** configuration, the slider axis is displaced by a distance $e$. 

### Position Analysis
The corrected theoretical model defines the slider displacement $x$ as a function of the crank angle $\theta$, crank radius $r$, connecting rod length $l$, and the vertical offset $e$:

$$x(\theta) = r \cos(\theta) + \sqrt{l^2 - (r \sin(\theta) - e)^2}$$

### Velocity & Acceleration
Taking the first and second time derivatives of the position equation with respect to time $t$ yields the velocity $v$ and acceleration $a$ profiles, where angular velocity $\omega = \frac{d\theta}{dt}$ and angular acceleration $\alpha = \frac{d\omega}{dt}$. The repository includes the computational scripts used to plot these dynamic profiles over a full rotation.

## 📁 Repository Structure
```text
├── CAD_Models/          # SolidWorks parts and assembly files (.SLDPRT, .SLDASM)
├── Math_Models/         # Computational scripts for plotting motion profiles
├── Documentation/       # Engineering drawings and theoretical correction notes
├── Media/               # Photos and videos of the physical prototype in motion
└── README.md
