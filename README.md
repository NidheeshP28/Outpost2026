# Bumper Goals - Custom RC Controller & Robot

An Arduino Nano-powered custom handheld remote controller and motorized robot system designed for the **Bumper Goals** project. This repository contains the controller firmware, hardware configurations, wiring guides, and design reference files.

## 🚀 Project Overview

### What it does
This project consists of two core systems: a custom handheld dual-joystick remote control transmitter and a motorized mobile robot chassis. The controller tracks micro-movements across two dual-axis joysticks simultaneously and maps them into directional instructions.

### How it works
* **The Controller:** A compact, Type-C USB Arduino Nano acts as the brain. The Nano monitors the varying analog voltages on pins `A0` through `A3` as the joysticks move. It translates these raw electrical inputs into integer coordinates from `0` to `1023` for smooth, proportional steering.
* **The Robot:** A separate receiver unit reads incoming control vectors and instructs its onboard motor drivers to actuate micro gearmotors, translating thumb movements into real-world agility.

### Why I made it
This system was built to provide a dedicated, highly ergonomic, and custom-tailored controller and chassis platform for tactical bumper sports. By crafting an independent custom controller rather than using bulky off-the-shelf gamepads, the internal mechanics, sizing, and balance are fully optimized.

---

## 🖼️ Media & Hardware Diagrams

### Project Simulation & Code Testing
The circuit and data translation are fully modeled and tested via online simulation before hardware assembly.

![Wokwi Simulation](WhatsApp%20Image%202026-07-09%20at%201.49.12%20PM.jpeg)

### Custom Hardware Enclosures & CAD Models
The project utilizes dedicated 3D-printed impact-resistant shells for both the remote control deck and the primary robotic body.

| Handheld Controller Case (Top Shell) | Internal Electronics Vault (Chassis Base) |
| :---: | :---: |
| ![Controller Shell](image_fbb8e9.png) | ![Chassis Base](image_fc0b85.png) |

| Assembled Robot Unit | Micro Gearmotor & Drivetrain Assembly |
| :---: | :---: |
| ![Full Robot Chassis](image_fc0ba3.png) | ![Gearbox Integration](image_fc0bc3.png) |

### Interactive PCB Layout
You can explore and inspect our hardware configuration and trace routes directly through your web browser:

[![View PCB on KiCanvas](https://hack.club/pcb-badge)](https://kicanvas.org/?github=https://github.com/<OWNER>/<REPOSITORY>/tree/main/pcb)

*(Note: Remember to replace `<OWNER>` and `<REPOSITORY>` in the link above with your actual GitHub username and repository name!)*

---

## 🛠️ Step-by-Step Build Guide

### Step 1: Prep your Electronics
Gather your components on a clean, static-safe workspace:
* **1x** Type-C USB Arduino Nano 3.0 (ATmega328P)
* **2x** Red Analog Joystick Modules (GND, +5V, VRX, VRY, SW)
* **1x** Premium hookup wire pack or breadboard jumper lines
* High-precision soldering kit or temporary prototyping breadboard

### Step 2: Physical Wire Routing & Assembly
Follow the pin configuration below to safely distribute power and signals from your sensors to the microcontroller core.

1. **Power Bus (VCC):** Connect the `+5V` pins of both red joysticks to the single `5V` output pin on your Arduino Nano. You can splice these into a shared junction line or run them into a mutual breadboard power rail.
2. **Grounding (GND):** Route the `GND` pins from both joysticks into the shared `GND` pins of your Nano to complete the electrical loops.
3. **Left Joystick Signal Lines:** Run a wire from the left joystick’s horizontal signal (`VRX`) pin to **A0** on the Nano, and its vertical signal (`VRY`) pin to **A1**.
4. **Right Joystick Signal Lines:** Run a wire from the right joystick’s horizontal signal (`VRX`) pin to **A2** on the Nano, and its vertical signal (`VRY`) pin to **A3**.
5. *Note: Leave the button switch (`SW`) pins on both joysticks completely empty/disconnected.*

### Step 3: Flash the Firmware
1. Hook up your physical Arduino Nano to your workstation via a **Type-C USB cable**.
2. Open your desktop **Arduino IDE**.
3. Copy the source code provided in `controller.ino` and paste it into a fresh project sketch window.
4. Navigate to **Tools > Board** and select **Arduino Nano**.
5. Navigate to **Tools > Processor** and ensure **ATmega328P** is chosen.
6. Choose your correct active port via **Tools > Port**.
7. Click the **Upload** icon (arrow symbol) to compile and burn the firmware onto your chip.

### Step 4: Final Mechanical Assembly
1. Open the **Serial Monitor** at a baud rate of `9600` to verify your live outputs (`0 - 1023`).
2. Once testing passes, slide the Arduino Nano and your wiring harness into the internal brackets inside the 3D-printed enclosure base (`image_fc0b85.png`).
3. Align and bolt down the dual joysticks into the faceplate recess using small metric machine hardware, then snap and secure the outer case shells together.

---

## 🔌 Pin Mapping (Wiring Configuration)

The physical and virtual devices map across the following digital and analog boundaries:
