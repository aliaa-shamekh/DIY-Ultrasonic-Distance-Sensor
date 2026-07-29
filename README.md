# DIY Ultrasonic Distance Measurement System 📏



## Overview

This project implements a distance measurement system using an ultrasonic sensor and an Arduino microcontroller.

The system measures the distance between the sensor and an object by sending ultrasonic waves, receiving the reflected signal, and calculating the distance based on the time taken for the echo to return.

## Features

* Real-time distance measurement
* Ultrasonic sensor interfacing with Arduino
* Serial monitor output for distance readings
* Simple and efficient embedded system design

## Hardware Components

* Arduino Uno / Arduino Nano
* HC-SR04 Ultrasonic Sensor
* Breadboard
* Jumper wires
* USB cable for programming and power

## How It Works

The ultrasonic sensor contains two main parts:

* **Trigger pin:** Sends an ultrasonic pulse toward the object.
* **Echo pin:** Receives the reflected wave.

The Arduino measures the time between sending and receiving the pulse, then calculates the distance using the speed of sound:

```
Distance = (Time × Speed of Sound) / 2
```

The division by 2 is required because the sound wave travels to the object and back.

## Circuit Connection

| HC-SR04 | Arduino        |
| ------- | -------------- |
| VCC     | 5V             |
| GND     | GND            |
| TRIG    | Digital Pin 9  |
| ECHO    | Digital Pin 10 |

## Software

* Arduino IDE
* C/C++ programming language

## Implementation

The Arduino continuously reads the sensor data and displays the measured distance through the Serial Monitor.

## Challenges & Debugging

During development, the sensor initially returned incorrect readings (`0 cm`). The issue was investigated by checking:

* Wiring connections
* Power supply stability
* Trigger pulse timing
* Echo signal response

After debugging the hardware and code, the sensor successfully produced accurate distance measurements.

## Skills Demonstrated

* Embedded Systems Development
* Arduino Programming
* Sensor Interfacing
* Hardware Debugging
* Circuit Connections
* C/C++ Programming

## Future Improvements

* Add an LCD/OLED display for standalone operation
* Improve measurement accuracy using filtering techniques
* Add object detection alerts using LEDs or a buzzer


## Project Credits 
*   **Developers:** Aliaa  Shamekh & Zeinab Mahmoud
*   **Academic Institution:** German International University (GIU) – Robotics and Automation
*   **Instructor:** Dr. Lobna Abo Serre.
