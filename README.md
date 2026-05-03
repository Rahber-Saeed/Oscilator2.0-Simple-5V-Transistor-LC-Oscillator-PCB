# Oscilator2.0-Simple-5V-Transistor-LC-Oscillator-PCB
A compact, self-oscillating LC circuit PCB designed in EasyEDA. Powers from 5V DC and utilizes a BC547 NPN transistor to generate oscillating signals. Includes PCB layout, 3D render, BOM, and pick &amp; place files. Perfect for learning basic oscillator electronics.
# Oscilator2.0 - Transistor LC Oscillator PCB

![EasyEDA](https://img.shields.io/badge/EasyEDA-v2.x-blue)
![License](https://img.shields.io/badge/License-MIT-green)

This repository contains the complete hardware design files for the **Oscilator2.0**, a simple, low-cost LC oscillator circuit designed using EasyEDA.

![Schematic](images/schematic.png)  <!-- Remember to actually place your schematic image in an 'images/' folder -->
![3D Render](images/3d_render.png) <!-- Place your 3D render image in 'images/' folder -->

## 📋 Project Description

The circuit uses a **BC547CTA** NPN bipolar junction transistor configured in a common-emitter/oscillator topology. The tank circuit comprises a **1mH** inductor and **22nF** capacitors to generate the oscillation. This is a great project for understanding fundamental radio frequency principles.


* **Power Input:** 5V DC (via 2-pin 5.00mm pitch connector)
<img width="1169" height="827" alt="Schematic_Oscilator2 0_2026-05-03" src="https://github.com/user-attachments/assets/c29686b1-aa11-4675-a922-f1489eee6f08" />

* **Key Component:** BC547CTA Transistor
<img width="586" height="692" alt="Oscilator2 0_3D_Top_View" src="https://github.com/user-attachments/assets/091a82fc-d4d0-4b04-ab2e-a146b0ac4ade" />

* **Output:** Oscillating signal (via a 2-pin header)
<img width="487" height="597" alt="Oscilator2 0_3D_Bottom_View" src="https://github.com/user-attachments/assets/24428eec-efed-44e7-892b-418abb304d84" />

* **Software:** EasyEDA / LCEDA
<img width="413" height="507" alt="Oscilator2 0_2D_View" src="https://github.com/user-attachments/assets/90999f00-29e7-41e2-ae95-5afea2e2c8e9" />





## 📂 Repository Structure

- 📁 **Images/** - Screenshots of the schematic, 2D PCB layout, and 3D render.
- 📄 **Schematic_Oscilator2.0_2026-05-03.pdf** - The full schematic in PDF format.
- 📄 **PCB_PCB_Oscilator2.0_2026-05-03.pdf** - The PCB layout visual.
- 📄 **BOM_Oscilator2.0_2026-05-03.csv** - Bill of Materials in CSV format.
- 📄 **PickAndPlace_PCB_Oscilator2.0_2026-05-03.csv** - Coordinates for automated assembly.

## 📦 Bill of Materials (BOM)

| ID | Name | Designator | Footprint | Quantity | Manufacturer (Part) | Notes |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | 0.1u | CB, CC | RAD-0.1 | 2 | - | Ceramic Capacitor |
| 2 | 1u | CE | RAD-0.1 | 1 | - | Ceramic Capacitor |
| 3 | 22n | CO1, CO2 | RAD-0.1 | 2 | - | Ceramic Capacitor (Tank Cap) |
| 4 | 2P-P5.00 | DCSOURCE, OUTPUT | CONN-TH_2P-P5.00 | 2 | - | 5mm Pitch Terminal Block |
| 5 | 1m | L1 | L_AXIAL-0.4 | 1 | - | Inductor (1mH) |
| 6 | BC547CTA | Q1 | TO-92-3 | 1 | onsemi | NPN Transistor |
| 7 | 10k | R1 | R_AXIAL-0.5 | 1 | - | Resistor |
| 8 | 4.7k | R2 | R_AXIAL-0.5 | 1 | - | Resistor |
| 9 | 2.2k | RC | R_AXIAL-0.5 | 1 | - | Resistor |
| 10 | 560 | RE | R_AXIAL-0.5 | 1 | - | Resistor |

*(Detailed prices and LCSC part numbers, where available, are in the CSV file)*

## 🔧 Assembly & Manufacturing

If you want to assemble this board via a service (like JLCPCB):

1. Use the **PCB_PCB_Oscilator2.0_2026-05-03.pdf** to verify tracks and holes.
2. Use the **PickAndPlace_PCB_Oscilator2.0_2026-05-03.csv** for component placement.
3. Check the **BOM_Oscilator2.0_2026-05-03.csv** for sourcing (available on LCSC).

## 🚀 How it Works

**Disclaimer:** *The circuit is named `Oscilator2.0` (missing an "l"). This is an intentional typo kept for project versioning consistency.*

This is a standard LC oscillator circuit. The frequency is determined by the inductor (L1) and the capacitors (CO1/CO2). The BC547 transistor provides the necessary gain to sustain the oscillation. Power is applied via the DCSOURCE connector.
