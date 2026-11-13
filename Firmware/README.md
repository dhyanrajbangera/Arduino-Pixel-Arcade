Arduino Controller Firmware

Four-Button Input System for Arduino Pixel Arcade

Overview

This directory contains the embedded firmware responsible for reading physical button inputs and transmitting directional commands to the browser-based arcade application.

The firmware is written in Arduino C/C++ and uses digital input pins configured with the internal pull-up resistors.

Hardware Configuration

The controller consists of four push buttons connected to the following digital pins:

Controller Direction| Arduino Digital Pin
Up| D2
Down| D3
Left| D4
Right| D5

Each push button connects its assigned digital pin to GND.

Firmware Specifications

Parameter| Configuration
Number of inputs| 4
Input mode| "INPUT_PULLUP"
Communication interface| USB Serial
Baud rate| 115200
Debounce interval| 25 ms
Output format| Directional character followed by newline

Communication Protocol

The firmware transmits a directional character when a button press is detected.

Physical Input| Transmitted Character
Up| "U"
Down| "D"
Left| "L"
Right| "R"

These commands are interpreted by the browser-based game through the Web Serial API.

Firmware Operation

1. Configure the four digital pins as inputs with internal pull-up resistors.
2. Initialize serial communication at 115200 baud.
3. Continuously monitor the button states.
4. Apply a 25 ms debounce interval.
5. Detect button press events.
6. Transmit the corresponding directional character.

Installation and Upload

1. Open "arduino_buttons.ino" in Arduino IDE.
2. Connect the Arduino-compatible board using USB.
3. Select the appropriate board and serial port.
4. Upload the firmware.
5. Connect the board to the computer running the arcade application.

Wiring Requirements

- Connect the Up button between D2 and GND.
- Connect the Down button between D3 and GND.
- Connect the Left button between D4 and GND.
- Connect the Right button between D5 and GND.

The firmware uses "INPUT_PULLUP", so external pull-up resistors are not required.

File Description

File| Description
"arduino_buttons.ino"| Main firmware for reading button inputs and transmitting serial commands.

System Integration

The firmware acts as the hardware input layer of Arduino Pixel Arcade. It converts physical button presses into serial commands that can be interpreted by the browser application.

This enables interaction with the arcade games through a dedicated physical controller.
