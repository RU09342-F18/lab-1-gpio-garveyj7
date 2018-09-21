# Multiple Blink
# What does this code do?
The programs control the blinking of the two LEDs on the MSP430G2553 and MSP430F5529.  However, both of these programs control the blinking differently.  Their functions are described below.

## For the MSP430G2553
### What does this code do?
This code makes the two LEDs on the board blink randomly and at different rates.  The length of the blinking can be controlled by the user.

### How does this code work?
This is achieved by using the rand() function.  This generates a random number everytime program loops.  If the number is even, the green LED lights up.  If the number is odd, the red LED lights up.  The speed of the blinks are controlled by the delay cycles function.

## For the MSP430F5529
### What does this code do?
This code blinks two LEDs by a user-defined period.  The rate of the blinking can be controlled by the user.  This can be done by adjusting the definitions of the individual LEDs.

### How does this code work?
The timer definitions are called "LED0Time" and "LED1Time".  LED0Time controls the green LED and LED1Time controls the red LED.  By adjusting the delay times, the user can make the two LEDs blink seperately in various patterns, or at the same time.

Two seperate counters are created to control the two LEDs.  These counters increment every time the program loops.  When the value of the counter exceeds the user-defined periods, the LEDs turn on and the counters are reset.

