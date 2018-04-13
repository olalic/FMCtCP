# What Are Make-Code Blocks really?

The goal of this exercise is to further understand the structure of programs, functions, and libraries. When thinking of make-code through a python lens, I view many of the make-code blocks to be functions that have been defined by the developers. Essentially that is what I understand libraries to be. In this post I developed three programs on make-code; a very simple one, a slightly more complex one, and finally a third program that does what the second one did, but uses a function I defined instead of one of the blocks that make-code has already created for us. This short chapter has the following learning goals: (1) in programming there are always multiple ways to get the same outcome, (2) you can use libraries that already exist if they include functions that do what you want them to do, or you may have to define you own function, (3) learn how to define a function in Python, (4) get an understanding of how make-code translates to Python.  

**The first program:**  The sole purpose of this program is to set all pixels to green. Though it is extremely simple, there is more happening ‘behind the blocks.’ For instance, make-code knows what the “set all pixels to” block wants the CPX to set its all of its pixes to a given color. This is because the function was previously defined and is called whenever I use the block. Similarly the block that is simply the color green, actually describes an RGB code: (0,255,0).

![Screen Shot 2018-03-12 at 7.40.35 PM](https://dcs102dot.files.wordpress.com/2018/03/screen-shot-2018-03-12-at-7-40-35-pm.png?w=248&h=279)

**The second program:**  This program is designed to change color when the sound level changes above a certain point. At first I defined the variable “Sound Level.” Then, in the forever loop the program sets all pixels to green if the sound level is below 2 and all pixels to yellow if the sound level is over or equal to 2.

![Screen Shot 2018-03-12 at 7.41.14 PM](https://dcs102dot.files.wordpress.com/2018/03/screen-shot-2018-03-12-at-7-41-14-pm.png?w=306&h=395)

**The third program:**  Finally, I use functions to re-create the pre-set blocks used in the second program. The two functions I defined are “set\_all\_lights\_to\_green” and “set\_all\_lights\_to\_yellow.” In each function, all ten pixels are told to turn green or yellow using a loop. Then in the forever loop I call the functions instead of using the “set all pixels to” block. Ideally this should demonstrate what blocks acutally are and how we can essentially create our own. The translation into Python below should make this point even more clear. 

![Screen Shot 2018-03-12 at 7.41.23 PM](https://dcs102dot.files.wordpress.com/2018/03/screen-shot-2018-03-12-at-7-41-23-pm.png?w=425&h=299)

**Translating the programs into Python**

**The first program translation**
```
from dcs import *

# On Start
setAllPixelsTo()

# Forever
while True:
  setAllPixelsTo(GREEN)
```

**The second and thrid program translation.** I have combined the translation for the second and thrid program, since the difference between the two was meant to highlight the ability to use and not use make-code blocks. In this case I just want to demonstrate how to translate what the two programs do into python. Slight differences in outcome are due to adjustments that needed to be made because the CPX doesn't have enough storage. 

```
#from dcs import *
from adafruit_circuitplayground.express import cpx

# This is the scaled, 0-100 function
from microphone import soundLevel, soundMagnitude
# Here's the setup instructions again
# http://lynxruf.us/courses/dcs102w18/cp/setup.html
import time

# Setup
def setAllPixelsToRGB (red = 0, green = 0, blue = 0):
    for i in range(10):
        cpx.pixels[i] = (red, green, blue)
cpx.pixels.brightness = 1

def pause (ms):
    time.sleep(ms / 1000.0)
    
# Forever
while True:
    reading = soundLevel()
    print(reading)
    if reading < 50:
        cpx.pixels[0] = (0,60,0)
    else:
        cpx.pixels[0] = (60,60,0)
    pause(50)
```

