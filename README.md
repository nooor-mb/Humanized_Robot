 # Humanized_Robot

Overview

This is a robotics project I built using Arduino. The robot can move forward when the ON/OFF button is pressed, detect obstacles with an ultrasonic sensor, speak using the VHM-314 SOP16 module, and rotate its head using a joystick-controlled servo. The project focuses on integrating electronics, sensors, motors, and simple mechanical movement in a beginner-friendly robotic system.

Purpose of the Project

The purpose of this project was to design and build a simple robotic system that demonstrates basic movement, obstacle detection, and human-robot interaction through sound and head rotation. It helped me learn wiring, Arduino programming, mechanical design limitations, and module integration.

Project Outcomes

A functioning robot capable of forward movement

Obstacle detection using ultrasonic sensor

Speech output using VHM-314 module + 3W speaker

Manual head rotation control using a joystick

Button-controlled movement for safe operation

Understanding of mechanical challenges, wiring management, and module communication

Features

Manual Movement: Robot moves only when the start button is pressed.

Ultrasonic Obstacle Detection: Stops the robot if an object is detected too close.

Voice Output: Plays audio using the VHM-314 speech module.

Rotating Head: Joystick controls servo rotation of the robot's head.

Controlled System: No automatic behavior—user controls all actions.

Setup Instructions
Hardware Setup

Connect motors to the motor driver (L298N or equivalent).

Wire the ultrasonic sensor to trigger/echo pins on Arduino.

Connect joystick module to analog pins (A0, A1).

Attach servo motor for head movement.

Connect the VHM-314 voice module to Arduino using serial pins.

Wire the ON/OFF button to a digital input pin.

Power the robot with a 7.4V battery or similar.

Follow your wiring diagram to assemble everything correctly.

Software Setup

Install Arduino IDE.

Install required libraries if needed (Servo.h, SoftwareSerial.h).

Open your .ino files:

Robot_Control.ino

Sensor_Module.ino

Head_Control.ino

Speech_Module.ino

Select board type (e.g., Arduino Uno) and correct COM port.

Upload all the code to the Arduino.

Usage Instructions
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

To replicate this robot:

Download the entire repository including code, diagrams, and photos.

Print or assemble the frame (if using 3D printed parts).

Follow wiring diagrams to attach motors, sensors, joystick, button, and speaker.

Upload the Arduino code from the Arduino_Code folder.

Mount all components securely on the robot frame.

Connect battery power and start testing movement, obstacle sensing, and head rotation.

Adjust wiring, sensors, and mechanical components as needed.

This ensures the robot works the same way as the original.

Functions and Methods
moveForward()

Moves the robot forward when the start button is pressed.

stopMotors()

Stops all movement when an obstacle is detected or button is off.

readDistance()

Reads ultrasonic sensor value.

speak(message)

Plays audio through VHM-314 module.

readJoystick()

Reads joystick input to rotate the head servo.

checkStartButton()

Reads button state to start/stop the robot.

File Format

.ino files for Arduino

.jpg photos of the robot

.png / .pdf wiring diagrams

.stl for any 3D printed parts

Input Validation

Debounce logic for button

Filtering and stabilization for ultrasonic readings

Smoothing joystick input to avoid shaky servo movement

Checking valid audio message numbers for VHM-314 module

Outputs and Test Cases
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

Issues Faced
1. Leg Mechanism Not Moving

The leg mechanism did not work as intended (no walking motion).
Reasons include:

Motors not strong enough

High joint friction

Poor alignment of leg parts

2. Robot Could Not Move Freely Due to Wiring

Movement was restricted because:

Many wires tangled during motion

Arduino, breadboard, and modules added heavy weight

Components were not fully fixed in stable positions

3. Leg Design Problems

Structure could not handle weight

Joints not smooth

Legs not balanced, causing the robot to tilt or get stuck

These issues prevented proper leg movement and natural motion.

Final Notes

This project gave me hands-on experience in robotics, wiring, Arduino programming, servo control, ultrasonic sensing, and integrating a voice module. Even though the leg mechanism and wiring created movement difficulties, the robot successfully demonstrated button-controlled motion, obstacle detection, head rotation, and audio output.
