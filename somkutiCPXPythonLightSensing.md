# Exploring Light Level Sensing on the CPX 
The following program explores the usage of the light sensor on the CPX using the DCS library in Python. 

Our code begins by importing all of the functions from the DCS library, giving us control over the CPX's various features

     from dcs import *
   

Then we setup our pixels to take commands, and initialize our variable light_reading that will hold the current level of light sensed by the CPX. We then get the current light level from the CPX using the function getLux() and store it in our variable light_reading.

    setupPixels()
    light_reading = 0
    light_reading = getLux() 

We want to be able to tell when our CPX senses a change in light level, so we  create a base state that will represent no change. 

In this case, our base state is when the LED's are at a 10 brightness and are the color red. The command setBrightness(_) allows us to change the brightness of all of our LED's at once. Similarly, the function setAllPixelstoRGB(x,x,x) allows us to change the colors of all of our LED's at once. This based upon the three input values in parentheses, which act as combinations of Red, Green, and Blue light. 

       setBrightness(10)    
       setAllPixelsToRGB(100,0,0)
    

If our light level changes, the brightness and colors of the LED's will change as well.  The following conditions are nested in a while loop that allows them to be checked constantly while the CPX senses light:
   

     while light_reading != 0:  
          light_reading = getLux()
          . . . conditions below . . .

Our first conditional statement is: 
if the light_reading is less than or equal to 50, set our pixel brightness to 75 and change our pixel color to green. 
  

     if (light_reading <= 50) :
                setBrightness(75)
                setAllPixelsToRGB(0,100,0)

Our second conditional statement is:
 if our light_reading is greater than 50 and less than 100, set our pixel brightness to 50 and our pixel color to blue.
  

     elif (light_reading > 50 and light_reading < 100):
                setBrightness(50)
                setAllPixelsToRGB(0,0,100)
          

Our last condition is: 
if none of our previous conditions are satisfied, set our pixel brightness back to 10 and our pixel color back to red.

       else:
             setBrightness(10)    
             setAllPixelsToRGB(100,0,0)
            
If the CPX still senses light, it then loops back to the beginning, updates the light_reading variable and checks all of the conditions again. 

So, we have created a program that changes the colors and brightness of the CPX LED's based on the level of light it senses!

One can view the program in its entirely below, and here is a [link](https://www.useloom.com/share/54eb3f7d62c543a8abab274ffa4f2579) to a screen cast explaining the script.

    from dcs import *
    #SomkutiLightSensor
    
    setupPixels()
    light_reading = 0
    light_reading = getLux() 
    
    setBrightness(10)    
    setAllPixelsToRGB(100,0,0)
    
    while light_reading != 0:  
          light_reading = getLux()
	      if (light_reading <= 50) :
                setBrightness(50)
                setAllPixelsToRGB(0,100,0)
		  elif (light_reading > 50 and light_reading < 100):
                setBrightness(25)
                setAllPixelsToRGB(0,0,100)
		  else:
	         setBrightness(10)    
             setAllPixelsToRGB(100,0,0)
