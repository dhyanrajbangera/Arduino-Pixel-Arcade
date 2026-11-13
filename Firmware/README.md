🔌 Arduino Controller Firmware

This folder contains the Arduino firmware used by the physical 4-button arcade controller.

📌 About

The firmware reads four physical push buttons and sends directional commands to the computer through USB Serial communication.

These commands are received by the browser-based arcade game to control gameplay.

🔧 Button Connections

Direction| Arduino Pin
Up| D2
Down| D3
Left| D4
Right| D5

⚙️ How It Works

- Uses four digital input pins.
- Configures the buttons using "INPUT_PULLUP".
- Detects button presses.
- Uses a 25 ms debounce delay.
- Sends directional characters through Serial communication.
- Sends data at a baud rate of 115200.

📡 Serial Commands

Button| Character Sent
Up| U
Down| D
Left| L
Right| R

Each command is transmitted with a newline character.

🚀 Upload Instructions

1. Open "arduino_buttons.ino" using Arduino IDE.
2. Connect your Arduino board to the computer.
3. Select the correct board and COM port.
4. Upload the firmware.
5. Connect the board to the computer running the arcade game.

🔌 Wiring Instructions

Each button should be connected between its assigned digital pin and GND.

The firmware uses the Arduino internal pull-up resistors, so external pull-up resistors are not required.

📂 File

- "arduino_buttons.ino" – Main Arduino firmware for the arcade controller.
