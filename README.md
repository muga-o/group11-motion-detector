//Project Overview
This project uses an Arduino Uno and a PIR motion sensor to detect movement. When motion is detected, a single LED lights up and a buzzer sounds to alert the user. When there is no motion, both the LED and buzzer remain off. This simple system can be used for basic security or automation alerts.

//Components Used
Component

Description

//Arduino Uno

Microcontroller to handle sensor and output

//PIR Motion Sensor

Detects infrared motion and sends signal

//Breadboard

For prototyping and connections

//LED (any color)

Lights up when motion is detected

//Buzzer

Sounds when motion is detected

//220Ω Resistor

Current limiting resistor for the LED

//Jumper Wires

Connect all components

//Circuit Connections
Device

//Arduino Pin / Connection

PIR Sensor VCC

Arduino 5V pin

PIR Sensor GND

Arduino GND pin

PIR Sensor OUT

Arduino Digital Pin 2

//LED Anode

Arduino Digital Pin 13 through 220Ω resistor

//LED Cathode

Breadboard Ground rail

Buzzer +

Arduino Digital Pin 12

Buzzer -

Breadboard Ground rail

Breadboard GND

Connected to Arduino GND

//How It Works
The PIR sensor continuously monitors for movement.
When motion is detected (PIR sensor output goes HIGH on pin 2):
The LED connected to pin 13 turns ON.
The buzzer connected to pin 12 sounds ON.
When no motion is detected (PIR sensor output is LOW):
The LED turns OFF.
The buzzer stops sounding.

//Usage Instructions
Connect the circuit according to the Circuit Connections table.
Upload the Arduino code to your Arduino Uno.
Open the Serial Monitor (baud rate 9600) to observe motion sensor outputs.
Move in front of the PIR sensor to trigger motion detection.
Observe the LED lighting up and buzzer sounding when motion is detected.
When no motion is detected, the LED and buzzer remain off.
Troubleshooting Tips
Double-check the polarity of the LED and buzzer.
Ensure resistors are connected in series with the LED.
Verify the common ground connection between the Arduino, PIR sensor, LED, and buzzer.
Test the buzzer and LED separately if they don’t respond.
Use the Serial Monitor output to verify if the PIR sensor is detecting motion.
