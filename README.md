# Smart-Latch-Controller
A button turns the system on. A motion sensor keeps it running. If no movement is detected for 30 seconds, it turns off automatically. An LED shows if it’s on.
# Soft-Latching-Power-System-With-Motion-Sensor

## 📘 Project Overview
This project showcases a smart power control system using an Arduino Uno, a PIR motion sensor, and a soft-latching technique. The system turns on with a button press, stays active as long as motion is detected, and automatically powers off after 30 seconds of inactivity. An LED indicates when the system is running. Ideal for energy-efficient applications like smart lighting or battery-powered devices.

---

## 🧰 Components Used

| Component         | Quantity | Description                                  |
|-------------------|----------|----------------------------------------------|
| Arduino Uno       | 1        | Microcontroller board                        |
| PIR Sensor        | 1        | Motion detection sensor                      |
| Push Button       | 1        | Trigger to start the system                  |
| NPN Transistor    | 1        | Controls the power latch                     |
| LED               | 1        | Shows system status                          |
| 220Ω Resistor     | 1        | Limits current to the LED                    |
| Jumper Wires      | As needed| For connections                             |
| Breadboard        | 1        | For prototyping                              |

---

## 🔌 Circuit Connections

### Push Button:
- One side → GND  
- Other side → Digital Pin D2 (with internal pull-up enabled)

### PIR Sensor:
- VCC → Arduino 5V  
- GND → Arduino GND  
- OUT → Digital Pin D3

### Transistor:
- Base → Digital Pin D5  
- Collector → Power line to load  
- Emitter → GND

### LED:
- Anode → 220Ω resistor → Digital Pin D13  
- Cathode → GND

---

## ⚙️ How It Works

1. When the button is pressed, the system powers on.
2. Motion resets the shutdown timer.
3. If no motion is detected for 30 seconds, the system shuts off.
4. LED indicates the current system status.

🎨 Designed by Aryam
