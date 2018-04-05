## My Simple MakeCode to Python Conversion
In this simple exercise, I have learned to convert a program from MakeCode into Python
## Here is my Python Code

from dcs import *
#on Start
light_Sensor=0
while True:
    light_Sensor=getLight
    print(light_Sensor)
    if light_Sensor>200:
        setAllPixelsTo(BLUE)
    else:
        setAllPixelsTo(GREEN)

## Here is my MakeCode

![enter image description here](https://lh3.googleusercontent.com/OX3A_zG3JIDm2fw4zLadl5mBlev2ajkR8_WkiK0zFJQ14R8YpUdUKCDsL3MF7Ik12QTtA3Dv7BNc "MakeCode")
