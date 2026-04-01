# 🔋 STM32 BlenderJet Controller

Embedded control and power management system for a portable blender using STM32.  
This project integrates battery charging, voltage regulation, and motor driving into a compact PCB design.

---

## 🚀 Features

- ⚡ **STM32 Microcontroller** for system control
- 🔋 **2S Li-ion Battery Charging** using TP5100
- 🔌 **LDO Regulation** for stable voltage supply
- ⚙️ **Motor Driver Circuit** for blender operation
- 🔧 **Programming Header (SWD)** for firmware upload
- 🧩 Modular schematic design (Power, MCU, Motor)

---

## 🧠 System Overview

The system is divided into the following blocks:

### 1. Power Management
- 5V input via USB
- TP5100 handles **2S battery charging**
- LC filtering for noise reduction
- LDO provides regulated output for STM32

### 2. Microcontroller (STM32)
- Handles system logic and control
- Interfaces with motor driver
- Supports SWD programming/debugging

### 3. Motor Driver
- Drives DC motor for blender
- Controlled via STM32 GPIO/PWM
- Includes protection and filtering components

---

## 🔌 Hardware Components

| Component | Description |
|----------|------------|
| STM32 MCU | Main controller |
| TP5100 | 2S Li-ion battery charger |
| LDO Regulator | Stable voltage output |
| Inductor + Capacitors | Power filtering |
| Motor Driver IC / MOSFET | Motor control |
| USB Input | 5V power source |

---

## 📷 Schematic

### Power + Charger + LDO
![Power Section](docs/power_schematic.png)

### STM32 + Motor Driver
![Control Section](docs/control_schematic.png)

---

## ⚙️ How It Works

1. 5V input is provided via USB  
2. TP5100 charges the 2S battery pack  
3. Output is filtered and regulated using LDO  
4. STM32 receives stable power  
5. STM32 controls the motor via driver circuit  

---

## 🛠️ Future Improvements

- Add **battery protection (BMS)**
- Implement **PWM speed control**
- Add **current sensing**
- Improve **EMI/EMC design**
- Optimize PCB layout for high current paths

---

## 📁 Repository Structure
├── docs/ # Images and diagrams
├── schematics/ # Circuit design files
├── pcb/ # PCB layout files
├── firmware/ # STM32 code (if added)
└── README.md

---

## 👨‍💻 Author

**Harsh Saini**  
Electronics & Communication Engineer  
Focus: Embedded Systems | Power Electronics | PCB Design  

---

## 📜 License

This project is open-source. Feel free to use and modify.

---

## ⭐ Support

If you found this useful, give it a ⭐ and share!
