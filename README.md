Arduino Pixel Arcade

A Browser-Based Retro Arcade with an Arduino-Powered Physical Controller

Arduino Pixel Arcade is an interactive retro gaming project that combines browser-based game development with physical hardware integration. It features ten arcade-style mini-games and supports both keyboard input and a custom four-button Arduino controller through the Web Serial API.

The project demonstrates the integration of embedded systems, web technologies, and human-computer interaction in a unified gaming platform.

Project Overview

The system consists of two primary components:

- Game Interface: A browser-based arcade application developed using HTML, CSS, and JavaScript.
- Physical Controller: An Arduino-based input system that reads four push buttons and transmits directional commands to the browser over USB serial communication.

Key Features

- Ten integrated arcade-style mini-games.
- Custom four-button physical controller.
- Browser-to-Arduino communication using the Web Serial API.
- Keyboard-based gameplay support.
- Retro-inspired graphical interface.
- Sound and music controls.
- Fullscreen gameplay support.
- Persistent high-score storage using browser local storage.

Game Collection

No.| Game| Gameplay Concept
01| Snake| Eat and grow while avoiding collisions.
02| Tetris| Arrange falling blocks to complete lines.
03| Breakout| Destroy bricks using a bouncing ball.
04| Flappy| Navigate through obstacles.
05| Pac-Man| Collect dots while avoiding enemies.
06| Donkey Kong| Climb platforms and avoid obstacles.
07| Frogger| Navigate across roads and rivers.
08| Space Invaders| Defend against incoming enemies.
09| Up & Down| Navigate between moving tracks.
10| Tapper| Serve customers across multiple counters.

Hardware Architecture

The physical controller uses four push buttons connected to digital input pins on an Arduino-compatible development board.

Controller Input| Arduino Pin
Up| D2
Down| D3
Left| D4
Right| D5

The firmware uses the internal pull-up configuration ("INPUT_PULLUP"). Each button is connected between its assigned digital pin and GND.

Software Architecture

Component| Technology
Game interface| HTML
Styling| CSS
Game logic| JavaScript
Hardware firmware| Arduino C/C++
Communication| Web Serial API
High-score storage| Browser Local Storage

Communication Protocol

The Arduino controller transmits directional characters over USB serial communication at 115200 baud.

Input| Serial Character
Up| "U"
Down| "D"
Left| "L"
Right| "R"

The browser reads these commands through the Web Serial API and uses them as gameplay inputs.

Getting Started

Requirements

- Arduino-compatible development board.
- Four push buttons.
- Jumper wires.
- USB cable.
- Arduino IDE.
- Google Chrome or Microsoft Edge with Web Serial support.

Installation and Setup

1. Clone the repository

git clone https://github.com/YOUR-USERNAME/Arduino-Pixel-Arcade.git

2. Upload the firmware

- Open "Firmware/arduino_buttons.ino" in Arduino IDE.
- Connect the Arduino board.
- Select the appropriate board and port.
- Upload the firmware.

3. Launch the game

- Open "Game/index.html" in a compatible browser.
- Connect the Arduino controller using the game's connection option.
- Select a mini-game and begin playing.

Keyboard controls remain available without the physical controller.

Keyboard Controls

Key| Function
Arrow Keys / WASD| Gameplay movement
M| Toggle sound
Escape| Return to the main menu

Menu navigation uses directional keys, with Right to select and Left to go back.

Repository Structure

Arduino-Pixel-Arcade/
│
├── README.md
│
├── Game/
│   ├── README.md
│   └── index.html
│
├── Firmware/
│   ├── README.md
│   └── arduino_buttons.ino
│
├── Images/
│   └── README.md
│
└── Documentation/
    └── README.md

Project Objectives

- Develop a multi-game browser-based arcade platform.
- Integrate physical hardware with a web application.
- Implement serial communication between an Arduino and a browser.
- Explore embedded programming and interactive system design.
- Demonstrate practical hardware-software integration.

Future Development

- Expand the physical controller with additional inputs.
- Introduce further arcade games.
- Improve controller ergonomics and enclosure design.
- Enhance the interface and gameplay experience.
- Expand technical documentation.

Project Status

The project includes a browser-based arcade application and Arduino firmware for a four-button controller.

---

Arduino Pixel Arcade
Combining retro gaming, embedded systems, and interactive technology.
