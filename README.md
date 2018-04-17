# CS207-Knock-Sensor-Lock
This repository explains how to build a Knock Sensor Lock using Arduino UNO.

# Introduction

This repository explains how to build a Knock Sensor Lock using an Arduino UNO. The lock system opens the lock when it hears a secret knock on the door. The system was installed on a cardboard house for demonstration purposes. The cardboard house has one entrance only, the main door. There are no other locks on the door other than the servo motor knock lock. The main door always remains locked and can only be unlocked by a secret knock. 
The working principle of the lock system is rather easy to understand. The knocks on the door are sensed by a Piezo buzzer. These knocks are then sent to the Arduino, where they are compared to a saved series of knocks in the system. Depending on whether the knocks match the knock series saved in the memory or not, the door stays locked or the door is unlocked by turning the servo motor. Every-time the door is unlocked, an audio recording is played to greet the user. 
There are two LED s and a push button attached to the wall on the inside of the house. One LED is green and the other one is red. These LEDs blink independently or in a sequence to represent many different processes of the system. The system also consists a push button, which is used to program a new knock series. This programming button replaces the knock series already saved in the memory, with the new series of knocks being recorded while the button is pressed.

# Parts and Tools needed
1 x Arduino UNO
1 x Piezo buzzer
1 x 1MΩ resistor
1 x Green LED
1 x Red LED
1 x Pushbutton
25 x 560Ω resistors
1 x 10kΩ resistor
1 x servo motor
4 x AA batteries
1 x Breadboard
Many assorted wires
Some cardboard boxes
Glue gun
Soldering iron
Battery-powered speaker
Box cutter
Computer to program the Arduino Board

# Team
Harpinder Singh Minhas

# Credits
Steve Hoefer - Grathio Labs - Programming Code
Alex James Clarke - University of Regina- Programming code
