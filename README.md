🎮 Arduino Pixel Arcade

A retro-style browser-based arcade featuring 10 classic mini-games, an Arduino-powered 4-button controller, and a custom interface using the Web Serial API.

🕹️ About the Project

Arduino Pixel Arcade brings classic arcade gaming together with physical hardware. Players can enjoy multiple mini-games directly in a web browser using either keyboard controls or a connected Arduino controller.

The project combines web development, Arduino programming, and hardware interaction to create an interactive gaming experience.

✨ Features

- 10 classic arcade mini-games
- Retro pixel-style interface
- Arduino-based 4-button controller
- Browser communication through the Web Serial API
- Keyboard controls
- Sound and music
- Fullscreen mode
- High-score tracking using browser local storage

🎯 Included Mini-Games

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

🔧 Hardware Components

- Arduino-compatible development board
- 4 push buttons
- Jumper wires
- USB cable
- Computer with a compatible browser

🔌 Controller Connections

Button| Arduino Pin
Up| D2
Down| D3
Left| D4
Right| D5

The firmware uses the Arduino "INPUT_PULLUP" configuration. Each button connects its assigned pin to GND when pressed.

💻 Software Requirements

- Google Chrome or Microsoft Edge for Web Serial support
- Arduino IDE
- USB connection to the Arduino controller

🚀 How to Run

1. Download or clone this repository.
2. Open the "Game" folder.
3. Open "index.html" in a compatible browser.
4. Connect the Arduino controller through USB.
5. Upload the firmware from the "Firmware" folder to your Arduino board.
6. Select the controller connection option in the game.
7. Start playing!

Note: Web Serial support is required for the physical controller. Keyboard controls can be used without connecting the Arduino.

🎮 Controls

Key| Action
Arrow Keys / WASD| Movement and gameplay
M| Toggle sound
Escape| Return to the game menu

Menu navigation uses the directional keys, with Right to select and Left to go back.

📁 Repository Structure

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

🧠 Technologies Used

- HTML
- CSS
- JavaScript
- Arduino
- C/C++
- Web Serial API

🎯 Project Objective

The objective of this project is to combine browser-based game development with physical hardware interaction, creating an accessible retro arcade experience using an Arduino-powered controller.

🔮 Future Improvements

- Add more arcade games
- Improve the physical controller design
- Add additional buttons and controls
- Improve the user interface
- Add more customization options

---

Developed as a hardware and software integration project.
