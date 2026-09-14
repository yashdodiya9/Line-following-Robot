# Line-Following-Robot

# The Line Follower — An Arduino-Based Autonomous Navigation Bot

A robust Arduino-powered robot engineered to autonomously follow a defined path using a five-sensor IR array and advanced feedback logic. This project demonstrates practical embedded systems design, real-time control, and creative automation, with an additional rear IR sensor for environmental interaction such as automated plant watering.

---

## Overview

This repository presents a fully documented **autonomous line-following robot** built on the Arduino UNO platform. The robot is designed to detect and track a black line on a white surface using a front-mounted array of five IR sensors, enabling precise path following, smooth curve negotiation, and reliable edge detection. An additional rear IR sensor is integrated to trigger auxiliary actions—such as activating a water pump for plant irrigation—when a specific marker is detected.

The project covers the complete development cycle: hardware assembly, sensor integration, embedded programming, and system testing.

---

## Key Features

- **High-Precision Line Tracking:** Utilizes a five-IR sensor array for accurate path detection and robust navigation, even on sharp curves.
- **Rear IR Sensor for Automation:** Dedicated rear sensor enables context-aware actions (e.g., watering plants when a marker is detected).
- **Differential Motor Control:** Employs an L298N motor driver for smooth, responsive movement and tight turns.
- **Modular, Expandable Design:** Easily adaptable for additional sensors (ultrasonic, Bluetooth, camera) and advanced behaviors.
- **Battery-Powered Mobility:** Operates untethered for real-world testing and demonstrations.

---

## Hardware Components

| Component             | Quantity | Description                                  |
|-----------------------|----------|----------------------------------------------|
| Arduino UNO R3        | 1        | Main microcontroller                         |
| IR Sensor Module      | 5 (front) + 1 (rear) | Line detection and rear automation      |
| L298N Motor Driver    | 1        | Dual H-bridge for DC motor control           |
| DC Gear Motors        | 2        | Drive wheels                                 |
| Robot Chassis         | 1        | Mounting platform                            |
| Wheels                | 2        | Standard 65mm                                |
| Caster Wheel          | 1        | Balance and support                          |
| Battery Pack          | 1        | 9V/12V or dual 18650 Li-ion cells            |
| Jumper Wires          | Several  | Circuit connections                          |
| Water Pump Module     | 1 (optional) | For plant watering automation           |

---

## Software & Tools

- Arduino IDE (v1.8+)
- Git/GitHub for version control
- Fritzing (optional, for circuit diagrams)
- Markdown editor for documentation

---

## System Architecture

1. **Sensor Array:** The five front IR sensors continuously monitor the track, providing granular feedback for left, right, and center alignment.
2. **Rear IR Sensor:** Detects a specific marker (e.g., black tape) to trigger the water pump or other actuators.
3. **Control Logic:** The Arduino processes sensor data in real time, adjusting motor speeds for accurate line following and executing auxiliary actions as needed.
4. **Motor Driver:** The L298N module receives control signals to drive the left and right motors independently, enabling smooth turns and corrections.

---

## Code Walkthrough

> File: `robot.ino`
## Components Walkthrough

> File: chasis

> File: Wheels

> File: Arduino Board and 5 IR Sensor Array

## Results

> File: `results.webm'

## How to Run
### Setup
> Clone the Repository
   ```bash
git clone https://github.com/yashdodiya9/Line-following-Robot.git

cd Line-following-Robot.git
