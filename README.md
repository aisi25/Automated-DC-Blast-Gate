I hired a professional several months ago to write this Arduino code to turn on/off dust collection system and open/close its blast gates
with Servos via a push buttons mounted on each tool in my workshop.

Before implementing this system I used to control the DC wirelessly with "PSI Woodworking LR2244 Long Ranger" and manually open/close the blast gates, and now the Arduino is using the same wireless controller to control the DC system and open/close the blast gates using servos mounted on each one with 3D printed mount and arm.

I used Servo Shield powered by 8A separate power supply for the Servos, and I used CAT 5e cable to wire the push buttons and the Servos to the Arduino.

In the beginning of using the system there was an issue where the some servos will become warm because the power is constantly provided to them and the Arduino trying keep each gate at the exact set angle while that is difficult to be done with such application, and this has been fixed by adding a relay to disconnect the power to the Shield after executing the command.
