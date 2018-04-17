# User Manual (How it works)
The functionality of each major component of this project is explained below:

## The Piezo buzzer
The Piezo buzzer is the ears of this project. When someone knocks on the front wall or the door, vibrations are created. These vibrations are converted into electricity by the Piezo buzzer. The buzzer then sends this electricity to the Arduino through wires. A 1MΩ resistor is added between the Arduino and Piezo buzzer to help the Arduino read incoming voltages from the Piezo buzzer. 

## Programming Button
The push button in this project is used to change and replace the knock saved in the memory. When the button is pressed, the system reads high voltage and goes into programming mode. In this mode, the user can knock up to a total of twenty knocks. Once a total of twenty are heard or the button is let go, the values from these new knocks replace the old values of the knocks; thus saving a new knock series or simply a new knock in the memory.

## The LEDs 
 The two LEDs blink on many occasions. Every time a knock is sensed the green led blinks once. If the knock matches, the green LED blinks three times, but if the knock does not match the red LED blinks three times instead. If a new knock series is programmed both green and red LEDs blinks three times together before blinking three more times one after another. These LEDs help the user understand what process the lock system is going through. 

## The Servo Motor
Once the door system receives power, the servo motor turns its lever to ninety degrees and keeps the door locked. When a knock matches, a signal is sent to the motor to turn its lever to zero degrees. Once at zero degrees, the servo motor no longer blocks the door which can easily be opened now. After six seconds pass the servo motor goes back to its locked position and blocks the door from being opened. The time servo motor keeps the door unlocked can be changed by changing the time in the programming code. 

## Battery powered speaker
After the servo motor unlocks the door and green LED blinks, an audio message is played on the battery powered speaker. A battery powered speaker is needed to play this sound because the Arduino does not provide enough current and voltage to play the message loud enough. An externally powered speaker plays the message loud enough to be easily heard.
