# CPS-Project-copy

Smart Coaster is a cyber-physical system prototype designed to remind the user to drink a hot beverage when its temperature is optimal.
The coaster monitors the temperature of a cup and notifies the user using LEDs, a buzzer melody, and Bluetooth communication.

This project was made as a course project for Cyber Physical Systems at Metropolia University of Applied Sciences.

---------------------------------------------------------------------------------------------------------------------------

System Architecture
  Arduino Uno (Slave)
    Reads sensors (TMP36, LDR)
    Controls LEDs and buzzer
    Sends data via HC-06 Bluetooth module
  ESP32 (Master)
    Sends data via HC-06 Bluetooth module
    Displays received data on a PC via USB serial

 Hardware Components
  - Arduino Uno
  - ESP32
  - HC-06 Bluetooth module
  - TMP36 temperature sensor
  - LDR (photoresistor)
  - 3 × LEDs (cold / medium / hot)
  - Buzzer
  - Resistors, wiring, power supply

---------------------------------------------------------------------------------------------------------------------------

How to Use

1. Power the Arduino Uno and ESP32
2. Place a hot beverage on the coaster
3. Observe LED indicators as the temperature changes
4. When the target temperature is reached:
  - The buzzer plays a melody
  - Temperature data is sent to the ESP32
5. Lift the cup to stop the alarm

---------------------------------------------------------------------------------------------------------------------------

Authors:
  Luukas, and two others