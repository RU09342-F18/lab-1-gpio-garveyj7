# Off Board Blink
## What does this code do?
The code "Multiple Blink" was uploaded onto the board before the MSP430 was removed.  This code was then run on the MSP430 on a breadboard as opposed to on the board.

## How was this accomplished?
The IC was removed off the board using an IC puller tool.  In order to make it work on a breadboard, a voltage of 3.3V was supplied to VCC.  Additionally, LEDs and 1K resistors were connected to ports 1.0 and 1.6.  The reset button was connected in the pull-up configuration using a 1nF capacitor and a 47k resistor.

## What does it look like?
When the power supply is turned on, the LEDs immediately start blinking as seen below.

![Alt Text](https://media.giphy.com/media/5dSVNUYGtB1rm80otW/giphy.gif)
