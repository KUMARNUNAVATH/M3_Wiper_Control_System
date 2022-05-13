# M3_Wiper_Control_System
We demonstrate a car wiper control system using the STM32F4xx-discovery board in this project. Most car wipers have a DC motor that controls their action, but the STM32F4xx-discovery does not have any motor, so we are considering LEDs for this application. As the wiper control system. There are four LEDs and a Push Button on the STM32F4xx-discovery board. These LEDs are orange, green, red, and blue in color. With the Discovery board, four user LEDs are connected to the PD12,PD13,PD14 and PD15 pins of PORTD through a current limiting resistor. GPIO pins of STM32F407VG microcontroller will be configured as digital input pins to enable a push button to operate with STM32F4. If you press the user button and hold it for two seconds, the Red LED turns on, indicating the ignition key is positioned at the ACC. In addition, the LEDs are blinking, which indicates the wipers are ON.

Wiper is ON: Initially, the wiper is off. On pressing the user input, Blue, Green, and Orange LEDs blink one at a time with the set frequency. The frequency changes with each alternate key press (key means push button). When the 1st key is pressed, the LED blinks at 1 sec per key, and when the 2nd key is pressed, the LED blinks at 0.25 sec per key press, and when the 3rd key is pressed, the LED blinks at 0.125 sec per key press. Wiper is OFF: Wiper is ON: The LED glow pattern stops after the fourth press; the wiper action begins after the second press onwards as explained in step 2. If the user button is pressed and held for 2 seconds, the red LED is off at the lock position

## In Action

1. user button and hold it for two seconds

 ![STM32 off](https://user-images.githubusercontent.com/101395036/167900171-dbeffc6e-24bb-4bba-a50d-663570184282.png)
 
2. On pressing the user input Alternating between three different frequency levels with 1, 4 and 8 Hz with every key press

![STM32F on 3LEDs](https://user-images.githubusercontent.com/101395036/168050686-654030f3-2c2a-47de-8d7e-8d2b179575b1.png)

3. user button is pressed and held for 2 seconds, the red LED is off
 
  ![STM32 trun OFF](https://user-images.githubusercontent.com/101395036/167905758-da67a99f-89f9-4507-8d52-5a76221d1ad0.png)

# BADGES
## codacy [![Codacy Badge](https://app.codacy.com/project/badge/Grade/580f6fc22d804e9aa29b4cfab0594707)](https://www.codacy.com/gh/KUMARNUNAVATH/M3_Wiper_Control_System/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=KUMARNUNAVATH/M3_Wiper_Control_System&amp;utm_campaign=Badge_Grade)
 
## Codiga ![code Quality Score](https://api.codiga.io/project/33315/score/svg)
 
## code Grade  ![code Grade](https://api.codiga.io/project/33315/status/svg)

## Build on linux [![Build-Linux](https://github.com/KUMARNUNAVATH/M3_Wiper_Control_System/actions/workflows/Build%20on%20linux.yml/badge.svg)](https://github.com/KUMARNUNAVATH/M3_Wiper_Control_System/actions/workflows/Build%20on%20linux.yml)
