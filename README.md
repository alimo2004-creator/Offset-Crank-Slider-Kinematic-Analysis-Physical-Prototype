# Offset Crank-Slider: Kinematic Analysis & Physical Prototype

![SolidWorks](https://img.shields.io/badge/SolidWorks-CAD-blue)
![Analysis](https://img.shields.io/badge/Analysis-SAM_7.0.97-success)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

## 🛠️ Tools & Technologies Used
* **Simulation:** SAM 7.0.97 (Mechanism Design Software)
* **CAD/CAM:** SolidWorks
* **Mathematical Modeling:** Analytical Kinematics, Offset Geometry Calculations
* **Fabrication:** Manual material fabrication and assembly

## ⚙️ How to Use This Repository
1. **Run the Simulation:** Download the `.sam` file from `Simulation_Files/` and open it in SAM 7.0 to view the node traces and dynamic graphs.
2. **Read the Report:** Open the PDF in the `Documentation/` folder for a deep dive into the transmission angles, dead-center calculations, and physical error analysis.
3. **View the Design:** Open the `.SLDASM` file in `CAD_Models/` to view the 3D assembly and its mechanical mates.

## 👨‍💻 Author
**Ali Mohamed Ahmed**
* Mechatronics & Robotics Engineering
* [LinkedIn](https://linkedin.com/in/ali-mohamed-ahmed) | [GitHub](https://github.com/alimo2004-creator)

## 📌 Project Overview
This repository contains the mathematical models, CAD files, and formal documentation for a physical model of an **offset crank-slider mechanism**. 

The primary objective of this project was to analyze the kinematic motion profiles (position, velocity, and acceleration) across a full 360-degree rotational cycle, confirm the quick-return characteristics of an offset configuration, and empirically validate the mathematical constraints using a fabricated physical prototype.

### ⚙️ System Parameters
The system was designed and evaluated using the following core dimensions:
* **Crank Length ($r$):** 55 mm
* **Coupler Length ($L$):** 145 mm
* **Offset Distance ($a$):** 65 mm

## 🚀 Key Features & Accomplishments
* **Kinematic Simulation:** Calculated peak velocity and acceleration profiles to evaluate the dynamic forces acting on the mechanism links, verified using SAM 7.0.97 simulation software.
* **CAD Modeling:** Designed a precise structural assembly in SolidWorks to ensure functional transmission angles and strict geometric alignment.
* **Physical Prototyping:** Fabricated and assembled the physical model to bridge the gap between theoretical calculations and real-world mechanical motion.
* **Empirical Evaluation:** Documented and analyzed mechanical losses in the physical build, specifically evaluating the impact of pin joint clearances and slider track friction on theoretical velocity curves.

## 📐 Mathematical Modeling
In a standard in-line crank-slider, the slider axis intersects the crank pivot. In this **offset** configuration, the slider axis is displaced by a vertical distance $a$. 

### Position Analysis
The theoretical model defines the slider displacement $x$ as a function of the crank angle $\theta$, crank radius $r$, connecting rod length $L$, and the vertical offset $a$:

$$x(\theta) = r \cos(\theta) + \sqrt{L^2 - (r \sin(\theta) + a)^2}$$

### Velocity & Acceleration
Taking the first and second time derivatives of the position equation with respect to time $t$ yields the velocity $v$ and acceleration $a$ profiles, where angular velocity $\omega = \frac{d\theta}{dt}$ and angular acceleration $\alpha = \frac{d\omega}{dt}$. The repository includes the computational scripts and analysis tables used to plot these dynamic profiles over a full rotation.


##
[📄 Read the Full Engineering Report (PDF)](Offset_Crank_Slider_Report.pdf)
[!cad_model](image.png)

## 📁 Repository Structure
```text
├── CAD_Models/          # SolidWorks parts and assembly files (.SLDPRT, .SLDASM)
├── Math_Models/         # Computational scripts for plotting motion profiles
├── Documentation/
│   └── Offset_Crank_Slider_Report.pdf  # Full kinematic analysis and project report
├── Media/               # Photos and videos of the physical prototype in motion
└── README.md
