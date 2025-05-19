 # 🤖 robotic_arm_rover

This is a **Robotic Arm Rover** project that combines mobility with a 6-DOF robotic arm, controlled wirelessly using NRF24L01 modules.

---

## 📌 Project Overview

The Robotic Arm Rover features:
- A powerful **motorized base** for mobility.
- A **multi-jointed robotic arm** for picking, placing, and manipulating objects.
- **Wireless communication** between a transmitter (remote) and a receiver (rover) using **NRF24L01** modules.
- Multiple control interfaces using joysticks, potentiometers, and switches.

This is an excellent robotics project for understanding wireless communication, servo control, arm kinematics, voltage regulation, and embedded programming.

---

## 🧰 Components Used

### 🔧 Electronics

| Component                                | Quantity |
|------------------------------------------|----------|
| Arduino Mega                             | 1        |
| Arduino Uno                              | 1        |
| NRF24L01 Wireless Module                 | 2        |
| NRF24L01 Power Adapter                   | 2        |
| 37mm DC Geared Motor (Reducer Motor)     | 2        |
| L298N Motor Driver (Green)               | 1        |
| MG996R / MG995 High Torque Servo         | 4        |
| MG90 Servo                               | 3        |
| Joystick Module                          | 2        |
| Potentiometer                            | 2        |
| Toggle Switch                            | 3        |
| 5mm LED + Resistors                      | 5 sets   |
| Mini Breadboard                          | 1        |
| LM2596 Step-Down Voltage Regulator       | 1        |
| 3S Li-po Battery                         | 1        |
| 18650 Li-ion Battery                     | 2        |
| Dual 18650 Battery Holder                | 1        |
| Jumper Wires                             | Various  |

### 🛠️ Mechanical

| Component                   | Quantity |
|-----------------------------|----------|
| 608 Bearings                | 4        |
| M8 60mm Bolts               | 2        |
| Anti-Loosening Nuts         | 2        |
| M3x6mm Bolts                | Various  |
| M3x10mm Bolts               | Various  |
| M3x14mm Bolts               | Various  |

---

## ⚙️ Working Principle

- The **transmitter unit** (Arduino Uno) sends control signals wirelessly via the NRF24L01 module.
- The **receiver unit** (Arduino Mega) receives these signals and actuates motors and servos accordingly.
- The rover moves using 37mm geared motors controlled by an L298N motor driver.
- A 6-DOF robotic arm (4x MG996R/MG995 + 3x MG90 servos) performs object manipulation.
- Joystick modules and potentiometers are used to control the direction, gripper, and arm joints.
- Toggle switches and LEDs add control modes and status indicators.
- Power is regulated using the LM2596 step-down regulator to safely power Arduino and servos from Li-ion or Li-po batteries.

---

## ✨ Features

- 📡 **NRF24L01 wireless communication** for long-range and low-latency control.
- 🦾 **6-DOF robotic arm** with high-torque servos.
- 🎮 Dual joystick and potentiometer interface for precise manual control.
- 🔋 Dual power supply options (3S Li-po or 18650 batteries).
- 🧠 Modular and scalable for additional sensors or automation.

---

## 🛠️ Assembly Steps

1. **Assemble the Robotic Arm & Chassis**  
   - Mount 37mm DC motors to the rover base.
   - Assemble the arm using MG996R/MG995 and MG90 servos.
   - Secure joints with 608 bearings and M3/M8 bolts.

2. **Wiring & Connections**  
   - Connect motor wires to L298N and servos to Arduino Mega.
   - Attach NRF24L01 modules using adapters for stable 3.3V power.
   - Hook up joysticks, potentiometers, and switches to Arduino Uno.

3. **Power Supply**  
   - Use the 3S Li-po to power motors via LM2596.
   - Use 18650 batteries for Arduino and logic circuits via voltage regulation.

4. **Upload Arduino Code**  
   - Upload `transmitter.ino` to Arduino Uno.
   - Upload `receiver.ino` to Arduino Mega.

---

## 📁 Folder Structure

Robotic-Arm-Rover/
│
├── transmitter/
│ └── transmitter.ino
├── receiver/
│ └── receiver.ino
├── images/
│ └── robotic_arm_view.jpg
├── diagrams/
│ └── wiring_diagram_transmitter.png
│ └── wiring_diagram_receiver.png
└── README.md


---

## 🔧 Future Enhancements

- Add Bluetooth or WiFi control with a mobile app.
- Integrate camera with object recognition using OpenCV.
- Add autonomous mode using ultrasonic sensors or LiDAR.
- Upgrade to brushless motors and smart ESCs for smoother motion.

---

## 📜 License

This project is open-source and free to use for educational and personal purposes. Please credit the original tutorial and contributors if shared publicly.

---








