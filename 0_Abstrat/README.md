# Wiper Control System
 We demonstrate a car wiper control system using the STM32F4xx-discovery board in this project. Most car wipers have a DC motor that controls their action, but the       STM32F4xx-discovery does not have any motor, so we are considering LEDs for this application. As the wiper control system.
There are four LEDs and a Push Button on the STM32F4xx-discovery board. These LEDs are orange, green, red, and blue in color. With the Discovery board, four user LEDs are connected to the PD12,PD13,PD14 and PD15 pins of PORTD through a current limiting resistor.
GPIO pins of STM32F407VG microcontroller will be configured as digital input pins to enable a push button to operate with STM32F4.
If you press the user button and hold it for two seconds, the Red LED turns on, indicating the ignition key is positioned at the ACC. In addition, the LEDs are blinking, which indicates the wipers are ON. 

Wiper is ON: Initially, the wiper is off. On pressing the user input, Blue, Green, and Orange LEDs blink one at a time with the set frequency. The frequency changes with each alternate key press (key means push button).
When the 1st key is pressed, the LED blinks at 1 sec per key, and when the 2nd key is pressed, the LED blinks at 0.25 sec per key press, and when the 3rd key is pressed, the LED blinks at 0.125 sec per key press.
Wiper is OFF: Wiper is ON: The LED glow pattern stops after the fourth press; the wiper action begins after the second press onwards as explained in step 2. If the user button is pressed and held for 2 seconds, the red LED is off at the lock position
