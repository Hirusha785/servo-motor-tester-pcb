# 🔧 Servo Motor Tester PCB

A compact PCB design for testing and controlling hobby servo motors using a 555 timer-based PWM signal generator. This project is designed for electronics learning, servo testing, prototyping, and basic embedded hardware experimentation.

---

## 📌 Project Overview

The **Servo Motor Tester PCB** allows users to generate a variable PWM signal to test standard servo motors without needing a microcontroller such as Arduino or ESP32. The circuit is based on the **NE555 timer IC**, with a potentiometer used to adjust the servo position by varying the pulse width.

This PCB is useful for checking servo motor movement, validating servo wiring, testing power connections, and learning basic PWM control concepts.

---

## ✨ Features

- 🔧 NE555-based PWM signal generation  
- 🎚️ Potentiometer control for servo position adjustment  
- 🔌 Dedicated 3-pin servo output connector  
- ⚡ 6V DC input supply connector  
- 💡 Power indicator LED  
- 🧩 Compact PCB layout  
- 🛠️ Beginner-friendly through-hole component design  
- 📐 Designed using KiCad  

---

## 🧠 How It Works

Servo motors are controlled using a PWM signal. A typical hobby servo expects a pulse every 20 ms, where the pulse width determines the motor position.

Typical servo control range:

| Pulse Width | Servo Position |
|------------|----------------|
| ~1.0 ms | 0° |
| ~1.5 ms | 90° |
| ~2.0 ms | 180° |

In this circuit, the **NE555 timer** works as an adjustable pulse generator. The potentiometer changes the timing resistance, which changes the output pulse width. This output signal is sent to the servo motor through the signal pin.

---

## 🧾 Components Used

| Reference | Component | Value / Type |
|----------|-----------|--------------|
| U1 | Timer IC | NE555P |
| RV1 | Potentiometer | 100kΩ |
| R1 | Resistor | 3.3kΩ |
| R2 | Resistor | 56kΩ |
| R3 | Resistor | 1kΩ |
| C1 | Capacitor | 22nF |
| D1 | Diode | 1N4148 |
| D2 | LED | Power Indicator |
| J1 | Power Connector | 2-pin input |
| J2 | Servo Connector | 3-pin output |

---

## 🔌 Pin Connections

### Power Input - J1

| Pin | Function |
|-----|----------|
| 1 | +6V DC |
| 2 | GND |

### Servo Output - J2

| Pin | Function |
|-----|----------|
| 1 | Signal |
| 2 | VCC |
| 3 | GND |

> ⚠️ Always verify the servo motor pinout before connecting. Different servo brands may use different wire color arrangements.

---
## 🖼️ Project Photos

### 1. Schematic Diagram

<img width="1368" height="538" alt="image" src="https://github.com/user-attachments/assets/cfaf9a5d-2d86-48a1-a397-da435bb6595d" />

![Servo Motor Tester PCB Layout](images/pcb-layout.png)

This schematic shows the NE555 timer-based PWM circuit, power input section, LED indicator, timing components, potentiometer, and servo output connector.

---

### 2. PCB Layout

<img width="866" height="806" alt="image" src="https://github.com/user-attachments/assets/b598e549-6842-4686-8bf2-60dddd74edbb" />

![Servo Motor Tester PCB Layout](images/pcb-layout.png)

This image shows the final routed PCB layout with component placement, traces, copper fill, connectors, mounting holes, and silkscreen labels.

---

### 3. 3D  View


<img width="606" height="641" alt="image" src="https://github.com/user-attachments/assets/84d22ae5-ea61-4fea-9c8c-d8e375e10370" />
<img width="1170" height="655" alt="image" src="https://github.com/user-attachments/assets/30e9959f-f44c-455f-a0ce-22b27bdadc6f" />
<img width="844" height="734" alt="image" src="https://github.com/user-attachments/assets/a12577ee-5930-411f-8120-1d02a3218bae" />
<img width="928" height="766" alt="image" src="https://github.com/user-attachments/assets/10f4d68e-8b25-43d4-9d56-2997560288fe" />

![Servo Motor Tester 3D Front View](images/3d-front-view.png)

This 3D view shows the completed PCB design with all through-hole components, including the NE555 IC, potentiometer, resistors, diode, capacitor, LED, and connectors.

---


---
## ⚡ Power Supply

Recommended input supply:

```text
6V DC
