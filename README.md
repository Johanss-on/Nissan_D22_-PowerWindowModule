# Arduino Car Power Windows Control

This project provides a solution for controlling the power windows of a car using an Arduino, a relay board, a push button, a 3-way toggle switch, and an LED. The LED flashes to indicate the active mode (which window is selected) whenever the mode changes or every 5 minutes. The push button is used to change the mode, and the toggle switch is used to roll the selected window(s) up or down.

## Components

- Arduino Uno [Model Number]
- 8-channel Relay Board [Model Number]
- Push Button [Model Number]
- 3-way Toggle Switch [Model Number]
- LED [Model Number]

## Wiring

- Relay Board: Connected to the Arduino's digital pins 2 through 9.
- Push Button: Connected to the Arduino's digital pin 10 and ground.
- Toggle Switch: Connected to the Arduino's digital pins 11 and 12 and ground.
- LED: Connected to the Arduino's digital pin 13.

## Operation

The system operates in six modes:

1. Front Left Window
2. Front Right Window
3. Both Front Windows
4. Rear Left Window
5. Rear Right Window
6. All Windows

Pressing the push button cycles through these modes. The current mode is indicated by the LED flashing a number of times corresponding to the mode number (once for mode 1, twice for mode 2, etc.).

The toggle switch has two positions. When it's in the down position, it rolls down the selected window(s). When it's in the up position, it rolls up the selected window(s).

## Code

The Arduino code for this project is included in the repository. It includes the functionality for controlling the power windows, changing modes with the push button, controlling the windows with the toggle switch, and indicating the active mode with the LED.

## Notes

Please ensure that your input pins are never left floating, as this can lead to unpredictable behavior. Pull-up or pull-down resistors are used to prevent this by ensuring the pin is always at a known voltage.

## Disclaimer

This project involves working with automotive electronics, which can be dangerous if not handled correctly. Always ensure that your circuits are properly protected and that you're mindful of the power requirements. If you're unsure about anything, it's best to consult with a professional.

## License

This project is licensed under the GNU License - see the LICENSE.md file for details.
