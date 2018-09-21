# Button Blink
## What does this code do?
This code turns on an LED when the user presses the button on the MSP430G2553 and MSP430F5529.  They both run a similar code, however, the pins are different.

## How does this code work?
The code detects the button press by performing an AND operation on the input register and button.  If this result is different than the resting state, the LED turns off.  When the button is released, the LED turns off, making the button momentary.
