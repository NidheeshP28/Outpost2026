# Bumper Goals - Custom RC Controller

An Arduino Nano-powered custom handheld controller designed for the **Bumper Goals** robotics project. This repository contains the controller's firmware, hardware setup configuration, and custom PCB designs.

## 🚀 Project Overview

### What it does
This controller acts as the handheld transmitter for a custom remote-controlled robot. It reads physical inputs from two analog joysticks simultaneously and processes the coordinates so they can be transmitted wirelessly.

### How it works
The system uses a compact, Type-C USB Arduino Nano as its brain. The Nano continuously samples the analog voltage changes on pins `A0` through `A3` as the joysticks move. It translates these electrical signals into a clean coordinate map ranging from `0` to `1023` for both the X and Y axes, allowing for smooth, proportional control over the robot's movement.

### Why I made it
This controller was built as a dedicated, lightweight, and ergonomic solution to drive the "Bumper Goals" mobile robot chassis. Instead of using a bulky, generic commercial controller, this custom setup allows for a tailored form factor that can fit into a compact, 3D-printed enclosure.

---

## 🖼️ Media & Diagrams

### Project Simulation
![Wokwi Simulation Screenshot]

### PCB Design
If you are viewing our hardware configuration, you can interact with the PCB layout directly:

[![View PCB on KiCanvas]

---

## 🛠️ Hardware Components
* **Microcontroller:** Type-C USB Nano 3.0 (ATmega328P compatible)
* **Inputs:** 2x Red Analog Joystick Modules
* **Enclosure:** Custom 3D-printed handheld case (In progress)

## 🔌 Pin Mapping (Wiring Configuration)
The joystick modules are connected to the Arduino Nano using the following layout:

### Joystick 1 (Left / Top)
* **VCC** -> Nano 5V
* **GND** -> Nano GND
* **VERT** -> Nano A1 (Vertical / Y-Axis)
* **HORZ** -> Nano A0 (Horizontal / X-Axis)

### Joystick 2 (Right / Bottom)
* **VCC** -> Nano 5V (Shared Line)
* **GND** -> Nano GND (Shared Line)
* **VERT** -> Nano A3 (Vertical / Y-Axis)
* **HORZ** -> Nano A2 (Horizontal / X-Axis)

## 📁 Repository Structure
* `controller.ino` - The firmware code that initializes the serial interface, reads analog pins, and processes joystick orientation.
* `diagram.json` - The Wokwi simulator diagram layout tracking the hardware configuration and physical wire routes.

## 💻 How to Test (Simulation)
1. Open the project files in [Wokwi Simulation](https://wokwi.com).
2. Click the green **Start Simulation** button.
3. Open the **Serial Monitor** tab to view the live coordinate stream (`0` to `1023`) as you manipulate the joysticks with your cursor.
