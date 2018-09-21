# Multiple Blink
For this lab, two different programs were created for the MSP430G2553 and MSP430F5529.  Both of these programs controlled the blinking of two LEDs on the MSP430s.

## MSP430G2553
The program on the MSP430G2553 blinks two LEDs randomly.  This is achieved by using the rand() function.  This generates a random number everytime program loops.  If the number is even, the green LED lights up.  If the number is odd, the red LED lights up.  The speed of the blinks are controlled by the delay cycles function.

## MSP430F5529
The program on the MSP430F5529 blinks two LEDs by a user-defined period.  These definitions are called "LED0Time" and "LED1Time".  LED0Time controls the green LED and LED1Time controls the red LED.  By adjusting the delay times, the user can make the two LEDs blink seperately in various patterns, or at the same time.

Two seperate counters are created to control the two LEDs.  These counters increment every time the program loops.  When the value of the counter exceeds the user-defined periods, the LEDs turn on and the counters are reset.
