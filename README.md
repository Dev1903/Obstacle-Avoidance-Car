# Obstacle-Avoidance-Car
## Overview

This project implements an obstacle avoidance car using Arduino and ultrasonic sensors. The car detects obstacles in its path and autonomously maneuvers to avoid them, ensuring smooth navigation in dynamic environments.

## Features

- **Obstacle Detection:** Uses ultrasonic sensors to detect obstacles in front and on the sides of the car.
- **Autonomous Navigation:** Automatically adjusts direction to avoid detected obstacles.
- **Servo-Controlled Steering:** Controls steering using a servo motor for precise maneuvering.
- **Motor Control:** Drives the car forward and backward based on obstacle detection.

## Components Used

- **Arduino Uno**: Microcontroller for sensor interfacing and motor control.
- **Sensors**:
  - Ultrasonic Sensor: Detects obstacles in front and on the sides of the car.
- **Actuators**:
  - DC Motors: Drive the wheels of the car.
  - Servo Motor: Controls steering.
- **Other**:
  - LED Indicators
  - Serial Monitor for debugging

## Circuit Diagram

### Pin Connections

- **Ultrasonic Sensor**: 
  - Trig pin: Analog pin A1
  - Echo pin: Analog pin A2
- **DC Motors**:
  - Left Motor Forward: Pin 7
  - Left Motor Backward: Pin 6
  - Right Motor Forward: Pin 4
  - Right Motor Backward: Pin 5
- **Servo Motor**: Pin 9

## Software Setup

### Libraries Required

- **Servo.h** (for controlling the Servo Motor)
- **NewPing.h** (for ultrasonic sensor function)

### Arduino Code

1. Include the necessary libraries (`Servo.h` and `NewPing.h`).
2. Define constants for pin mappings and sensor parameters.
3. Implement setup to initialize sensors and actuators.
4. Create a loop to continuously read sensor values, detect obstacles, and control the car's movement accordingly.

### Adjustments

- **Obstacle Detection Logic**: Modify the obstacle avoidance algorithm based on specific sensor readings and car maneuverability.
- **Sensor Calibration**: Calibrate sensors as needed to ensure accurate obstacle detection and avoidance.

## Operation

The car operates as follows:

- **Obstacle Detection**: Uses ultrasonic sensors to measure distances and detect obstacles.
- **Autonomous Navigation**: Adjusts direction autonomously to avoid obstacles.
- **Steering Control**: Uses a servo motor to steer the car and DC motors to drive it forward or backward.

## Usage

1. Connect sensors and actuators according to the provided pin connections.
2. Upload the Arduino sketch to the Arduino Uno board.
3. Monitor sensor readings and system operation via the Serial Monitor.
4. Test the car in various environments to ensure effective obstacle avoidance.
