Smart Door Lock with Passcode
Description
This Arduino-based smart door lock project simulates a fingerprint scanner using buttons and adds passcode entry via the serial monitor. It uses an LCD display for status messages and a servo motor to control the door lock mechanism.

Hardware Requirements
Arduino board (e.g., Uno)
16x2 I2C LCD display
Servo motor
2 push buttons
Jumper wires
Breadboard (optional)
Software Requirements
Arduino IDE
Libraries: Wire.h, LiquidCrystal_I2C.h, Servo.h (install via Arduino Library Manager if needed)
Pin Connections
LCD: SDA to A4, SCL to A5 (I2C)
Servo: Signal to pin 9
Correct Fingerprint Button: Pin 7
Wrong Fingerprint Button: Pin 8
Setup Instructions
Connect the hardware as per the pin connections above.
Open the Arduino IDE and upload the provided code (smart_door_lock.ino).
Open the Serial Monitor (Tools > Serial Monitor) and set baud rate to 9600.
Usage
Fingerprint Simulation: Press the correct button (pin 7) to simulate a valid fingerprint and unlock the door. Press the wrong button (pin 8) for an invalid attempt.
Passcode Entry: In the Serial Monitor, type 1234 and press Enter to unlock the door. Any other input will display an error.
The LCD will show status messages, and the servo will rotate to 90° to unlock for 3 seconds, then return to 0° (locked).
Notes
Ensure the LCD address is correct (0x3F in the code; may vary).
The door locks automatically after opening.
This is a simulation; add real sensors (e.g., fingerprint module) for a complete system.


Copy message
