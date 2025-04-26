# Arduino Reflex Game (8-Button "Spede" Clone)

This project is an Arduino-based reflex game inspired by Peten Paja's "Spede" game.  
It uses 8 buttons, 8 LEDs, a 4-digit TM1637 display, and a buzzer for sound effects.  
You can test your reaction speed, challenge your friends, and keep track of the high score!

## Features

- **8-Button Gameplay:** Test your reflexes with 8 buttons and corresponding LEDs.
- **4-Digit Score Display:** See your score in real time on a TM1637 display.
- **High Score Saving:** High scores are stored in EEPROM (non-volatile memory).
- **Sound Effects:** Feedback sounds for correct, wrong, and game over events.
- **High Score Reset:** Hold all buttons for 2 seconds to reset the high score.
- **Mute Option:** (Optional) Add a physical switch to turn sound ON/OFF.

## Hardware Requirements

- **Arduino Mega 2560** (other models with enough pins should also work)
- **8 Push Buttons**
- **8 LEDs** (with resistors)
- **TM1637 4-Digit 7-Segment Display Module**
- **Buzzer or Speaker**
- **(Optional) 74HC595 Shift Register** (for custom digit multiplexing, can be removed if only TM1637 is used)
- **(Optional) Mute Switch**
- Jumper wires, breadboard or PCB

## Pinout

- **Buttons:** Pins 30–37
- **LEDs:** Pins 22–29
- **TM1637 Display:** CLK (Pin 4), DIO (Pin 5)
- **Buzzer/Speaker:** Pin 2
- **(Optional) Shift Register:** Latch (7), Clock (8), Data (9)
- **Digit Enable (Optional):** Pins 10, 11, 12, 13

## How to Play

1. **Start the Game:** Press any button to start.
2. **React Quickly:** When a LED lights up, press the corresponding button as fast as you can!
3. **Score:** Each correct press increases your score and speeds up the game.
4. **Game Over:** Press the wrong button or be too slow—the game ends.
5. **High Score:** Try to beat your high score!  
   Hold all 8 buttons for 2 seconds to reset the high score.
6. **(Optional) Mute:** If you add a mute switch, flip it to turn sounds on or off.

## Getting Started

1. **Connect your hardware** according to the pinout above.
2. **Install Arduino libraries:**
    - [TM1637Display](https://github.com/avishorp/TM1637)
3. **Upload the code** from `reflex_game.ino` to your Arduino Mega.
4. **Open the Serial Monitor** (9600 baud) to see debug messages.

## Acknowledgments

- Original idea and inspiration: [Peten Paja's Spede Project](http://petenpaja.blogspot.com/2013/04/first-project-arduino-spede.html?m=1)

## License

This project is open source. See the `LICENSE` file for details.
