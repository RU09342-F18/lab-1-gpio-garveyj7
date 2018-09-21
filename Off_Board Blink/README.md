# Off Board Blink
The code "Multiple Blink" was uploaded onto the board before the MSP430 was removed.

The IC was removed off the board using an IC puller tool.  In order to make it work on a breadboard, a voltage of 3.3V was supplied to VCC.  Additionally, LEDs and 1K resistors were connected to ports 1.0 and 1.6.  The reset button was connected in the pull-up configuration using a 1nF capacitor and a 47k resistor.

When the power supply was turned on, the LEDs immediately started blinking as seen below.

![Alt Text](https://media.giphy.com/media/5dSVNUYGtB1rm80otW/giphy.gif)
