I hired a professional several months ago to write this Arduino code to turn on/off dust collection system and open/close its blast gates
with Servos via a push buttons mounted on each tool in my workshop.

Before implementing this system I used to control the DC wirelessly with "PSI Woodworking LR2244 Long Ranger" and manually open/close the blast gates, and now the Arduino is using the same wireless controller to control the DC system and open/close the blast gates using servos mounted on each one with 3D printed parts (attached) .

I used Servo Shield powered by separate 8A power supply for the Servos, and I used CAT 5e network cable to wire the push buttons and the Servos to the Arduino.

In the beginning of using the system the servo driver/shield MOSFET burnt out when I connect all the servos because is not designed for continuous power for more than 3 parallel servos, and the solution was to bypass it. (attached)

And also there was an issue where the some servos will become warm because the power is constantly provided to them and the Arduino trying keep each gate at the exact set angle while that is difficult to be done in such application, and this has been fixed by adding a relay to disconnect the power to the Shield after executing the command.

The 3D printed servo mount has a place for a micro limit switch wired to green & red LEDs to indicate the gate status physically


Main Parts:

Arduino UNO R3

SunFounder PCA9685 16 Channel 12 Bit PWM Servo Driver

DS3218 servo 20KG Full Metal Gear 25T Servo

25T Servo Horn

Momentary Hinge Roller Lever Micro Limit Mini Switch (https://www.amazon.com/gp/product/B06XFL4MZ2/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1)

4in Self-Cleaning Metal Blast Gate

PSI Woodworking LR2244 Long Ranger




Thank You.
