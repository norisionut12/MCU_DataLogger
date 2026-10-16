# ⚡ MCU DataLogger – PCB Design

A compact **data logger board** built around the **ATmega328P**, the same chip that powers the Arduino Uno. It reads sensors, keeps track of the exact date and time, and saves everything to on-board memory, so it can log data on its own without a computer.

🛠️ **My part:** I recreated the schematic of an existing circuit in **KiCad 10** and designed the complete PCB for it, from component placement to routing.

<p align="center">
  <img src="Images/Screenshot%202026-10-16%20113004.png" alt="3D view – top" width="650">
</p>

## 🔍 What's on the board

| | |
|---|---|
| 🧠 **ATmega328P** | The brain of the board, running at 16 MHz |
| ⏰ **DS1337 clock** | Keeps the date and time, so every reading gets a timestamp |
| 💾 **2 × 24LC1025 memory** | 256 KB of storage that keeps the data even without power |
| 🔌 **Connectors** | Sensors (D2–D8), I²C, serial (RX/TX), programming (ICSP) and battery |

## 📐 Schematic

Redrawn in KiCad from the original circuit and organized into clear blocks: clock, MCU, memory and connectors.

<img src="Images/Screenshot%202026-10-16%20113028.png" alt="Schematic" width="100%">

<details>
<summary>Connectors sheet</summary>
<br>
<img src="Images/Screenshot%202026-10-16%20113036.png" alt="Connectors sheet" width="400">
</details>

## 🟩 PCB

A 2-layer board with ground fill on both sides. The crystals sit right next to their chips to keep the signals clean, and all connectors are placed on the edges.

| Component placement | Routing (red = top, blue = bottom) |
|:---:|:---:|
| <img src="Images/Screenshot%202026-10-16%20112928.png" width="400"> | <img src="Images/Screenshot%202026-10-16%20112942.png" width="400"> |

| 3D – top | 3D – bottom |
|:---:|:---:|
| <img src="Images/Screenshot%202026-10-16%20113004.png" width="400"> | <img src="Images/Screenshot%202026-10-16%20113012.png" width="400"> |

## 📂 Open the project

Open `MCU_DataLogger.kicad_pro` in **KiCad 10** or newer.

> 🚧 The board is fully designed but has not been manufactured yet.
