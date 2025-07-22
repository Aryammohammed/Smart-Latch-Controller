# Smart-Latch-Controller
A button turns the system on. A motion sensor keeps it running. If no movement is detected for 30 seconds, it turns off automatically. An LED shows if it’s on.
📘 Project Overview
This project presents a power-saving control system using a pushbutton and a PIR motion sensor. When the button is pressed, the system powers on and remains active as long as motion is detected. If no movement is detected for 30 seconds, the system automatically shuts down. An LED indicates when the system is active. It's ideal for low-power embedded designs and automation projects.

🧰 Components Used
Component	Quantity	Description
Arduino Uno	1	Main microcontroller board
PIR Sensor	1	Passive Infrared sensor for motion detection
Push Button	1	Manual trigger to power the system on
NPN Transistor	1	Used to latch power to parts of the system
LED	1	Indicates when the system is active
220Ω Resistor	1	Current limiter for LED
Jumper Wires	As needed	For making all circuit connections
Breadboard	1	For building the prototype
🔌 Circuit Connections
Button:
One side → GND

Other side → Digital Pin D2 with INPUT_PULLUP

PIR Sensor:
VCC → Arduino 5V

GND → Arduino GND

OUT → Digital Pin D3

Transistor:
Gate/Base → Digital Pin D5

Collector → Circuit Power Line

Emitter → GND (through load or switch)

LED Indicator:
Anode → 220Ω resistor → Digital Pin D13

Cathode → GND

⚙️ How It Works
User presses the button → system turns on.

As long as motion is detected, the system remains powered.

If no motion is detected for 30 seconds, the system shuts down.

The LED provides a clear visual cue for system activity.

🎨 Designed by Aryam 
