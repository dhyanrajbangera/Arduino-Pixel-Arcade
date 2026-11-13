Arduino-powered retro pixel arcade featuring 10 mini-games, a custom 4-button controller, and browser-based gameplay using the Web Serial API.
🕹️ Arduino Pixel Arcade

An Arduino-powered retro arcade featuring 10 classic-style mini-games, pixel-art graphics, sound effects, and a physical four-button controller.

The project connects an Arduino button controller to a browser-based arcade using the Web Serial API.

🎮 About the Project

Arduino Pixel Arcade combines browser-based game development with physical hardware.

Players can navigate the arcade and play games using either keyboard controls or a custom Arduino-based four-button controller.

The browser game is built with HTML, CSS, and JavaScript, while the Arduino firmware reads physical button inputs and sends directional commands to the browser over USB Serial.

✨ Features

- 10 playable mini-games
- Retro pixel-art graphics
- Animated game selection menu
- Sound effects and background music
- Fullscreen gameplay
- High-score tracking in the browser
- Keyboard controls
- Physical Arduino four-button controller
- USB Serial communication using the Web Serial API

🕹️ Mini-Games

1. Snake
2. Tetris
3. Breakout
4. Flappy
5. Pac-Man
6. Donkey Kong
7. Frogger
8. Space Invaders
9. Up & Down
10. Tapper

🔧 Hardware

- Arduino-compatible microcontroller
- 4 push buttons
- USB cable
- Connecting wires

🔌 Controller Connections

Button| Arduino Pin| Direction
Button 1| D2| Up
Button 2| D3| Down
Button 3| D4| Left
Button 4| D5| Right

The firmware uses the Arduino internal pull-up resistors, so each button connects between its assigned pin and GND.

💻 Software and Technologies

- HTML
- CSS
- JavaScript
- Arduino C++
- Web Serial API
- USB Serial Communication

🚀 How to Run

1. Upload the Arduino Firmware

1. Open the firmware file in the Arduino IDE.
2. Select your connected Arduino board and port.
3. Upload the firmware.

2. Open the Arcade

1. Open the game HTML file in a browser that supports the Web Serial API, such as Chrome or Edge.
2. Click CONNECT in the arcade.
3. Select your Arduino device when prompted.
4. Use the physical buttons to control the games.

You can also play using the keyboard.

🎹 Keyboard Controls

Key| Action
Arrow Up / W| Up
Arrow Down / S| Down
Arrow Left / A| Left
Arrow Right / D| Right
M| Toggle sound
Escape| Return to menu

📁 Repository Structure

Arduino-Pixel-Arcade/
│
├── README.md
│
├── Game/
│   └── index.html
│
├── Firmware/
│   └── arduino_buttons.ino
│
├── Images/
│   └── README.md
│
└── Documentation/
    └── README.md

🎯 Project Goal

The goal of this project is to combine software development, embedded systems, and interactive game design into one arcade experience.

It demonstrates how physical hardware can interact with browser-based software through serial communication.

🔮 Future Improvements

- Add more arcade games.
- Design a custom 3D-printed controller enclosure.
- Improve the physical controller design.
- Add more interactive hardware features.
- Enhance the arcade interface and gameplay.

---

Project: Arduino Pixel Arcade
Platform: Browser + Arduino
Controller: Four-button USB Serial controller
