# 🤖 Arduino Dual Servo Motor Control

![Project Setup](./7BB6488B-90FA-4F65-A2AF-FDA04DDBAFFC.jpeg)

This project demonstrates how to control two micro servo motors using an Arduino Uno board. It is suitable for beginners who are exploring motor control, PWM signals, and Arduino programming.

## 🔌 Components Used
- Arduino Uno R3
- 2x Micro Servo Motors (SG90 or similar)
- Jumper Wires
- USB cable (for power and programming)

## 🔧 Wiring
Each servo motor has 3 wires:
- **Brown or Black** – GND
- **Red** – VCC (5V)
- **Orange or Yellow** – Signal (PWM)

### Connections:
- **Left Servo Motor**:
  - Signal → Digital Pin 9
  - VCC → 5V
  - GND → GND

- **Right Servo Motor**:
  - Signal → Digital Pin 10
  - VCC → 5V
  - GND → GND

## 🧠 Arduino Code Sample
```cpp
#include <Servo.h>

Servo servo1;
Servo servo2;

void setup() {
  servo1.attach(9);  // Attach to pin 9
  servo2.attach(10); // Attach to pin 10
}

void loop() {
  servo1.write(0);
  servo2.write(180);
  delay(1000);

  servo1.write(180);
  servo2.write(0);
  delay(1000);
}
```

## 🎯 Purpose
This setup can be used in:
- Robotic arms
- Remote-controlled systems
- Educational demos for motion control

## 📅 Year
2025 – All rights reserved © Arduino Project
