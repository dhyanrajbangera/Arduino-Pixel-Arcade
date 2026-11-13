Game Application

Browser-Based Arcade Interface

Overview

This directory contains the main software component of Arduino Pixel Arcade. The application is a browser-based retro gaming platform featuring ten integrated mini-games.

Developed using HTML, CSS, and JavaScript, the application provides the graphical interface, game logic, input handling, and communication interface for the external Arduino controller.

Features

- Ten arcade-style mini-games.
- Retro-inspired graphical interface.
- Keyboard-based input.
- Arduino controller integration.
- Web Serial communication.
- Sound and music controls.
- Fullscreen functionality.
- High-score persistence through browser local storage.

Included Games

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

Input Methods

Keyboard Input

Input| Function
Arrow Keys / WASD| Gameplay movement
M| Toggle sound
Escape| Return to menu

Arduino Controller

The application supports a four-button Arduino controller through the browser's Web Serial API.

The expected serial communication speed is 115200 baud.

Serial Character| Input
U| Up
D| Down
L| Left
R| Right

Execution

1. Open "index.html" using Google Chrome or Microsoft Edge.
2. Connect the Arduino controller through USB if hardware input is required.
3. Use the application's controller connection option.
4. Select a game from the main menu.

Compatibility: The physical controller requires browser support for the Web Serial API. Keyboard gameplay does not require an Arduino connection.

File Description

File| Description
"index.html"| Main arcade application containing the interface, styling, and game logic.

Integration

The game application communicates with the Arduino firmware through USB serial communication. Incoming directional commands are interpreted as controller inputs during gameplay.
