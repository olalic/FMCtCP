# “Constrain” Block Exploration

This is the block "Constrain" in the "Math" section in MakeCode. It gives you 3 spaces to add variables/numbers etc. The first space is where you put the variable you want to constrain, and the next 2 spaces are where you put in the numbers to indicate a range within which you want to constrain the first variable. For example, "constrain X between 1 and 10" means to constrain the variable X within the range between 1~10, anywhere outside the range will be invalid and will not be "X".

## **Program 1: Just set a variable**

<div style="position:relative;height:calc(300px + 5em);width:100%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.adafruit.com/---codeembed#pub:_ERAgAm8XrFb3" allowfullscreen="allowfullscreen" frameborder="0" sandbox="allow-scripts allow-same-origin"></iframe></div>

Python Code:
		      
		      def constrain (value, min, max)
		        If value < min
		          Result = min
		        If value > max
		          Result = max
		        Return result 

This program uses “constrain” as the definition for a new variable to limit its value within a set of range. Firstly, I still use “light” as the initial variable set as input light level which varies as CPX measures light intensity of the environment. Then I set the second variable “limited light” with “constrain ‘light level’ between 100 and 200”. That means the variable new “limited light” only measures and displays light level within the boundary I set between 100 and 200.

## **Program 2: Different light for different range**

<div style="position:relative;height:calc(300px + 5em);width:100%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.adafruit.com/---codeembed#pub:_7Ju37EYEYiwi" allowfullscreen="allowfullscreen" frameborder="0" sandbox="allow-scripts allow-same-origin"></iframe></div>


Python Code:
		      
	def constrain (value, min, max)
		if value < min
			Result = min
		if value > max
			Result = max
		Return result 
		
	Light_level = getLux( )
	Limited_light = constrain (light level, 100, 200)

	if Limited_light == Light_level:
		setAllPixelsTo(GREEN)
	else:
		setAllPixelsTo(RED)


This program grows from program 1 to let CPX respond to the light level measured differently depends on whether if it lies within or outside the “constrain” I set for “limited light”. The “if” statement can be a little confusing since it sets a relationship between 2 interrelating variables “light” and “limited light”. However, it simply means that I ask the CPX to measure “light” which is the environment’s light intensity and compare it to the range of 100~200 that I set for “limited light”. If light level lies within that range, then all pixels will turn green, otherwise all pixels will turn blue.

(Important side note here: the position of “light” and “limited light” doesn’t matter. Because either block will end up measuring the same input which is light intensity. As long as there is a logical correlation established between the two, the CPX will read the light intensity and comparing it to the set range for “limited light” and respond accordingly).

## **Program 3: Actually useful program monitoring the range of temperature of freezer**

<div style="position:relative;height:calc(300px + 5em);width:100%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.adafruit.com/---codeembed#pub:_gYk1bm7pxh97" allowfullscreen="allowfullscreen" frameborder="0" sandbox="allow-scripts allow-same-origin"></iframe></div>

Python Code:
		      
	Siren        = 0
	Powerup		= 1

	def playSound (Sound = Siren)
		if Sound == Siren 
			cpx.play_file("siren.wav")
		elif Sound == Powerup
			cpx.play_file("powerup.wav")

	def constrain (value, min, max)
		if value < min
			Result = min
		if value > max
			Result = max
		Return result 
	
	Temperature = getTemperatureC ( )
	Freezer_Temperature = constrain (Temperature, -4, 4)

	if Freezer_Temperature == Temperature: 
		setAllPixelsTo(GREEN)
	else:
		setAllPixelsTo(RED)
		playSound (Siren)



This program is a similar one to program two but it is actually useful in daily life. I used it to measure another input which is temperature. I first set a variable “temperature” which varies with the temperature detected by the CPX. Then I set a range of -4~4 ºC for a new variable “freezer temperature” using “constrain” which corresponds to the range of temperature I want my freezer to be at. Using the same logic “if…then…” statement to see if the “temperature” lies within the range of “freezer temperature”. If the temperature lies within the range, all pixels turn green and signals normal function of freezing. If not, the sound “siren” will be played and all pixels will turn red to double-alert someone to check it out. I also added another block to stop all the sound if button A is clicked. That is to prevent the people fixing the freezer gets too irritated by the sound (which could be probably after 5 seconds) and smash the CPX.
