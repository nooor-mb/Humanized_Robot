 # Humanized_Robot


# Overview

This is a robotics project I built using Arduino. The robot can move forward when the ON/OFF button is pressed, detect obstacles with an ultrasonic sensor, speak using the VHM-314 SOP16 module, and rotate its head using a joystick-controlled servo. The project focuses on integrating electronics, sensors, motors, and simple mechanical movement in a beginner-friendly robotic system.


# Purpose of the Project

The purpose of this project was to design and build a simple robotic system that demonstrates basic movement, obstacle detection, and human-robot interaction through sound and head rotation. It helped me learn wiring, Arduino programming, mechanical design limitations, and module integration.


# Project Outcomes

Achieved controlled movement using an ON/OFF button.

Obstacle detection using ultrasonic sensor

Speech output using VHM-314 module + 3W speaker

Manual head rotation control using a joystick


# Features

Manual Movement: Robot moves only when the start button is pressed.

Ultrasonic Obstacle Detection: Stops the robot if an object is detected too close.

Voice Output: Plays audio using the VHM-314 speech module.

Rotating Head: Joystick controls servo rotation of the robot's head.

Controlled System: No automatic behavior—user controls all actions.

# Setup Instructions

Technical Components Used

Arduino board

Ultrasonic sensor (for distance measurement)

Motors 

ON/OFF button

Joystick module for head rotation

Wires, breadboard, battery

Basic frame and legs (manual structure)



# Software Setup

Install Arduino IDE.

Install required libraries (Servo.h, SoftwareSerial.h).

Select board type (e.g., Arduino Uno) and correct COM port.

Upload all the code to the Arduino.

# Usage Instructions
Start Movement

Press the ON/OFF button

Robot begins moving forward

Obstacle Detection

If the ultrasonic sensor detects an obstacle within ~20cm

Robot stops and plays audio

Rotate the Head

Move the joystick left/right

Servo rotates the robot’s head smoothly

Play Voice Messages

The VHM-314 module plays audio when speak() is triggered in the code

Stop Movement

Press the ON/OFF button again

Robot immediately stops

Replication of the Project


# Outputs and Test Cases
Test 1: Start Movement

Input: Press button
Expected: Robot moves forward

Test 2: Ultrasonic Obstacle Detection

Input: Place object close
Expected: Robot stops + audio plays

Test 3: Joystick Head Rotation

Input: Move joystick
Expected: Head rotates smoothly

Test 4: Voice Module Output

Input: Trigger speak()
Expected: Speaker plays sound

Test 5: Stop Robot

Input: Press button again
Expected: Robot stops

# Issues Faced
1. Leg Mechanism Not Moving

The leg mechanism did not work as intended (no walking motion).
Reasons include:

Motors not strong enough

High joint friction

Poor alignment of leg parts

2. Leg Design Problems

Structure could not handle weight

Joints not smooth

Legs not balanced, causing the robot to tilt or get stuck

These issues prevented proper leg movement and natural motion.

3. Robot Could Not Move Freely Due to Wiring

Movement was restricted because:

Many wires tangled during motion

Arduino, breadboard, and modules added heavy weight

Components were not fully fixed in stable positions


# Conclusion

This project introduced the fundamental concepts of robotics, including sensor control, manual movement activation, and mechanical design. Although the robot faced challenges such as leg movement limitations and wiring interference, it still demonstrated successful obstacle detection and head rotation through a joystick. The project helped build a strong understanding of Arduino-based control systems and provided a clear path for future improvements in design and motion mechanics.
