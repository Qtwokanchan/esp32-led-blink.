# ESP32 GPIO LED Control

## 📝 Overview
A foundational embedded systems project demonstrating GPIO manipulation using an ESP32. This simulation establishes basic digital output control, showcasing how microcontroller logic interfaces with and drives physical hardware peripherals.

## 🛠️ Hardware & Tools
* **Microcontroller:** ESP32
* **Components:** 1x Standard LED (Red), 1x 220Ω Resistor, Jumper wires
* **Simulation Environment:** Wokwi
* **Languages:** Embedded C

## ⚡ Circuit Schematic & Wiring
> **Note:** [Upload your Wokwi screenshot here]

### Pin Mapping
| Component | Microcontroller Pin | Function |
| :--- | :--- | :--- |
| LED Anode | GPIO 14 | Digital Output (3.3V Logic) |
| LED Cathode | GND (via 220Ω Resistor) | Current Limiting |

## ⚙️ How It Works
* **Hardware Logic:** A 220-ohm resistor is placed in series with the LED. This is critical for limiting the forward current and protecting the LED from drawing excess current from the microcontroller pin, which could damage both components.
* **Control Logic:** The ESP32 is programmed to configure GPIO 14 as an output pin. The embedded C code utilizes a continuous loop to drive the pin `HIGH` (outputting 3.3V) and `LOW` (outputting 0V) at 1-second intervals, creating a steady blink cycle.

## 🚀 How to Simulate
1. Open the Wokwi Simulation: [Paste your Wokwi project link here]
2. Click the "Play" button in the simulator.
3. Observe the LED cycling between active and inactive states based on the programmed delay.

## 🧠 Engineering Learnings
* Configured general-purpose input/output (GPIO) pins for digital signaling.
* Translated software instructions (Embedded C) into physical electrical state changes.
* Applied fundamental circuit protection principles using current-limiting resistors in a digital logic circuit.
* 
