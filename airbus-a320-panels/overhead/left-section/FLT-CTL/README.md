# OpenA3XX – FLT CTL Panel (CPT) v1.0  
**Flight Simulation Hardware – Flight Control Panel (Captain Side)**

---

## 🧭 Overview

This panel replicates the **Flight Control (FLT CTL)** section of the Airbus OpenA3XX cockpit for the captain’s side. It provides toggle control and status indication for flight control computers:

- **ELAC1** (Elevator Aileron Computer)
- **SEC1** (Spoiler Elevator Computer)
- **FAC1** (Flight Augmentation Computer)

Each computer function is represented by a Korry-style push-button switch with integrated illumination.

> ⚠️ **Flight Simulation Only – Not for use in real aviation applications.**

---

## 🖼️ Panel Layout

The FLT CTL (CPT) panel features a single-row layout:

- **ELAC1**, **SEC1**, **FAC1** (Left to Right)
  - Each module includes:
    - Dual push-button Korry-style switch with `FAULT` and `OFF` indicators.
    - Silkscreen-labeled frames for switch position.
    - LED illumination zones surrounding each module.

The panel is labeled with "FLT CTL" across the top and individual legends above each switch position.

---

## 🛠️ PCB Details

### 🔌 Connectors & Interfaces

#### J1 – 10-pin Header (Top Right)
- Interface header positioned for ribbon cable access.
- Silk labels indicate pin numbers (1–10).

#### K1–K3 – Korry Switch Connectors
- 4-pin headers for each of the three modules:
  - **K1** – ELAC1
  - **K2** – SEC1
  - **K3** – FAC1
- Clearly labeled silkscreen and positioned below each switch cutout.

---

### 💡 LEDs and Indicators

- 18 yellow surface-mount LEDs (D1–D18), distributed as follows:
  - 6 LEDs per Korry module zone.
  - Positioned for consistent backlighting around switches.

#### Resistors
- Current-limiting resistors (R1–R6) for LED power regulation.

---

### 🧷 Mounting and Assembly

- 2 mounting holes, one on each side for enclosure or frame fitting.
- Front panel silkscreen includes:
  - Module boundaries
  - Labeling for component alignment
  - Pin orientation for each connector

---

## ⚙️ Fabrication and Panel Fit

This PCB is designed for integration with an external **acrylic front panel** that includes:
- Cutouts for 3 rectangular Korry-style switches.
- Engraved legends: `ELAC1`, `SEC1`, `FAC1`, and `FLT CTL`.
- Alignment with LED backlighting zones.

PCB size and cutouts match standard OpenA3XX dimensions for MIP compatibility.

---

## 🔗 Attribution

- **Version**: FLT CTL (CPT) Panel v1.0  
- **Project**: [OpenA3XX](https://www.github.com/OpenA3XX)  
- **License**: CC BY-SA 4.0  
- **Note**: Design for simulation use only.
