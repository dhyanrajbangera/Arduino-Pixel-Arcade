🎮 Game – Arduino Pixel Arcade

This folder contains the main browser-based arcade game.

📌 About

The game is developed using HTML, CSS, and JavaScript. It features a retro pixel-style interface with 10 different mini-games.

Players can interact with the games using keyboard controls or a connected Arduino controller through the Web Serial API.

🎯 Included Games

- Snake
- Tetris
- Breakout
- Flappy
- Pac-Man
- Donkey Kong
- Frogger
- Space Invaders
- Up & Down
- Tapper

✨ Features

- Retro arcade interface
- Multiple mini-games
- Keyboard input
- Arduino controller support
- Sound and music
- Fullscreen mode
- High-score saving

🚀 How to Run

1. Open "index.html" in Google Chrome or Microsoft Edge.
2. Select a game from the main menu.
3. Use the keyboard to play.
4. Connect the Arduino controller to use physical buttons.

🎮 Controls

Key| Function
Arrow Keys / WASD| Movement
M| Toggle sound
Escape| Return to menu

📂 File

- "index.html" – Main arcade game containing the game interface and gameplay code.

🔗 Hardware Integration

The game communicates with the Arduino controller using the Web Serial API at 115200 baud.

The controller sends directional commands to the browser when its buttons are pressed.
