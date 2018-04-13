# Simple Program

In changing the simple code from makecode to python, I stuck with the same idea, therefore I just had to translate the blocks to written code. The “from dcs import” allows us to have the colors defined as “RED” and “BLUE”, and the sensors defined for us. Then I initiate the sound sensor variable, so the CPX will react to the sound sensor, and create the if/ else statement that says if the sound that the CPX hears is equal to than 155 then it sets all of the Pixels to red. It executes the same program as makecode, but it does it through python.**
## Python
from dcs import *

#On Start

sound_Sensor=0

#Forever

While True:
    sound_Sensor=getSound
    print(sound_Sensor)
    if sound_Sensor=155
        setAllPixelsTo(RED)
## Makecode



# Slightly more Complex Program

I did the same thing as the simple code and added and else statement.
## Python

from dcs import *

#On Start

sound_Sensor=0

#Forever

While True:
    sound_Sensor=getSound
    print(accel_x_reading)
    if sound_Sensor=155
        setAllPixelsTo(RED)
    else
        setAllPixelsTo(BLUE)
  ## Makecode 
  
# More Complex or Different Program

For the do it differently code I struggled a bit because I was unsure of how to program the CPX with the button being pressed. I set it up as a true/ false program where if button A was pressed the value was 1 and if button A was not pressed the value was 0. Then I wrote an if/else statement that had Blue lights turned on when button A was pressed and red lights when button A was not pressed.

## Python
from dcs import *

#On Start

button_A=1

#Forever

While True:
    button_A=getbutton
    print(buttonA)
    if button_A=1
        setAllPixelsTo(RED)
    else
	setAllPixelsTo(BLUE)
	 ## Makecode
 

    
