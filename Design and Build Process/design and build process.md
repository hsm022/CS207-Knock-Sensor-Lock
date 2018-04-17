# Design Process
Simplicity and usability were kept in mind while creating the project. The house to demonstrate the lock was made out of cardboard. The only way to enter the house is through the front door, which can only be unlocked by the secret knock. Four pieces of cardboard were used to make the structure of the house. Two pieces for the side walls, one for the front wall and the fourth piece for the roof. A door was shaped and cut out of the front wall. This cut piece of cardboard was then taped to the front wall from the inside to make it look like a door. 
Now on the inside of the safe house, a little box was attached to one of the side walls and the front wall. This box was made to hide the power source, the Arduino UNO board and many other little parts of the lock system. A green LED, a red LED and a push button were attached to the outside of this little box to help the user operate the lock system. Another cardboard platform was glued on to the front wall to hold the battery powered speaker. The last thing that was attached to the front wall was the Piezo buzzer.

The legs of the LED s and the push buttons were poked through the visible side of the little cardboard box which holds the power source and the Arduino. Different coloured wires were soldered to the legs of these LEDs and the push button, which were then attached to the Arduino at a later stage.


 To connect the Piezo buzzer, a slightly different approach was used. The legs of the Piezo buzzer were pushed through a somewhat thinner piece of cardboard because the legs were short. These legs were then soldered to two wires which were connected to the Arduino. The thin cardboard with the Piezo buzzer was then glued to the front wall. 

At last a very little box was attached to the door. This box was made for the servo motor lever to lock or unlock the door. The lever from the servo motor lever rests in this little box and keeps the door locked by blocking the door. When a command is sent to unlock the door, the servo motor turns its lever, thus unblocks or in other words, unlocks the door. 

# Build Process
The circuit for this system has many different things attached to the breadboard and is quite complex to grasp all at once. In order to better understand, the build process has been divided into small steps of connecting the major parts of the project one by one.


## The Piezo buzzer
For this project, the two wires coming from the Piezo buzzer were connected to the 1MΩ resistor on a breadboard, then one wire from the resistor was connected to a ground pin and the other one was connected to the analog pin A0 of the Arduino board.

## Push Button
The soldered wire from one leg of the button was connected to 5volts on the breadboard. The other leg was connected to the ground with a 10kΩ resistor in between the button and ground. A third wire was attached between the resistor and the button. The other end of this third wire was connected to the digital pin 8 set as input to read high or low voltages.

## Green and Red LEDs
The two LEDs in this project work following the same circuit design. The circuit design of an LED is quite easy to build. The soldered wire from the positive leg of the LED was attached to a digital output pin of the Arduino. The other leg was connected to a 560Ω resistor, which was then connected to the ground. In this project, the green LED is attached to digital pin 11 and the red LED is connected to digital pin 12.

## Servo Motor
The servo motor has three wires brown, red and yellow. The brown wire goes to the ground, the red wire goes to 5Volts. The third wire or the yellow wire is used to give the servo motor different commands. For this project, the yellow wire was attached to digital output pin 13.


## Battery powered speaker

Since the ordered parts were not received, the only way left to play an audio was to use some of the Arduino’s memory. To play the audio saved in the memory, the digital signals from the Arduino needed to be             R/2R Ladder Circuit [4]
turned into analog signals. The R/2R ladder circuit was used to do this. This circuit required twenty-five 560Ω resistors and eight wires connected to Arduino digital output pins from 0 to 7. The auxiliary cable from the speaker was connected to the circuit by connecting one end of the auxiliary cable to output from R/2R ladder circuit and the ground. 
