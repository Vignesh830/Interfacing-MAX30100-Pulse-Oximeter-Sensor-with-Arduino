# Interfacing-MAX30100-Pulse-Oximeter-Sensor-with-Arduino
In this project we will be Interfacing MAX30100 Pulse Oximeter Sensor with Arduino. The MAX30100 Sensor is capable of measuring Blood Oxygen & Heart Rate. We can use any display like a 16×2 LCD Display to view the value of SpO2 and BPM. The blood Oxygen Concentration termed SpO2 is measured in Percentage and Heart Beat/Pulse Rate is measured in BPM.

How does Pulse Oximeter Works?
Oxygen enters the lungs and then is passed on into blood. The blood carries oxygen to the various organs in our body. The main way oxygen is carried in our blood is by means of hemoglobin. During a pulse oximetry reading, a small clamp-like device is placed on a finger, earlobe, or toe.
![1](https://github.com/Vignesh830/Interfacing-MAX30100-Pulse-Oximeter-Sensor-with-Arduino/assets/159744719/380e6eda-40d7-4fcb-83fd-f4b10b703c6a)
Small beams of light pass through the blood in the finger, measuring the amount of oxygen. It does this by measuring changes in light absorption in oxygenated or deoxygenated blood.
![2](https://github.com/Vignesh830/Interfacing-MAX30100-Pulse-Oximeter-Sensor-with-Arduino/assets/159744719/e2ecd0b1-f7c2-4ae2-b044-f1ccbce4a27a)

Features

1. Consumes very low power (operates from 1.8V and 3.3V)
2. Ultra-Low Shutdown Current (0.7µA, typ)
3. Fast Data Output Capability
4. Interface Type: I2C

Working of MAX30100 Pulse Oximeter and Heart-Rate Sensor

The device has two LEDs, one emitting red light, another emitting infrared light. For pulse rate, only infrared light is needed. Both red light and infrared light are used to measure oxygen levels in the blood.

When the heart pumps blood, there is an increase in oxygenated blood as a result of having more blood. As the heart relaxes, the volume of oxygenated blood also decreases. By knowing the time between the increase and decrease of oxygenated blood, the pulse rate is determined.
It turns out, oxygenated blood absorbs more infrared light and passes more red light while deoxygenated blood absorbs red light and passes more infrared light. This is the main function of the MAX30100: it reads the absorption levels for both light sources and stores them in a buffer that can be read via I2C communication protocol.

Interfacing MAX30100 Pulse Oximeter Sensor with Arduino

Now let us interface MAX30100 Pulse Oximeter Sensor with Arduino and display the value in serial monitor.The circuit diagram and connection is very simple. You can follow the same.
![Interfacing-MAX30100-Pulse-Oximeter-Sensor-with-Arduino-1](https://github.com/Vignesh830/Interfacing-MAX30100-Pulse-Oximeter-Sensor-with-Arduino/assets/159744719/8de2cd1d-d5c7-4891-88e9-09019c4dcab9)
Connect the Vin pin of MAX30100 to Arduino 5V or 3.3V pin, GND to GND. Connect the I2C Pin of MAX30100, i.e SCL & SDA to A5 & A4 of Arduino.
Source Code/Program

The source Code/program for interfacing MAX30100 Pulse Oximeter with Arduino is written in C programm for Arduino IDE. This code will display the value in serial monitor. Copy this code and upload it to Arduino Board.

