# Simple blink on a MSP430G2553 and a MSP(FILL IN WHAT BOARD YOU ARE USING)

## What does this code do?
This code was designed to make an LED blink for a defined interval of time.  

## How does this code work?
In order to accomplish this task, the pin that controls the LED had to be defined.  As seen in the data sheet, the LED is controlled by port 1.0.  A ‘for’ loop containing a ‘_delay_cycles()’ function was used to blink the LED.  

This function delays the clock cycles for a user-defined amount of time and repeats indefinitely (as there are no conditions in the for loop).  In order to switch the LED on and off, the loop XOR’s the output status of LED, switching it on and off after every loop is completed.

### The _delay_cycles() function
‘_delay_cycles(x)’ hauls the code and waits for x cycles before resuming.  For example, If the user was running the MSP430 at 1 MHz and wanted a 1 second blink, they would use ‘_delay_cycles(1000000)’.
