# “Constrain” Block Exploration

This is the block "Constrain" in the "Math" section in MakeCode. It gives you 3 spaces to add variables/numbers etc. The first space is where you put the variable you want to constrain, and the next 2 spaces are where you put in the numbers to indicate a range within which you want to constrain the first variable. For example, "constrain X between 1 and 10" means to constrain the variable X within the range between 1~10, anywhere outside the range will be invalid and will not be "X".

## **Program 1: Just set a variable**

[https://makecode.com/_eHdCzgK1KbAv](https://makecode.com/_eHdCzgK1KbAv)

This program uses “constrain” as the definition for a new variable to limit its value within a set of range. Firstly, I still use “light” as the initial variable set as input light level which varies as CPX measures light intensity of the environment. Then I set the second variable “limited light” with “constrain ‘light level’ between 100 and 200”. That means the variable new “limited light” only measures and displays light level within the boundary I set between 100 and 200.

## **Program 2: Different light for different range**

[https://makecode.com/_HUJegAdug71V](https://makecode.com/_HUJegAdug71V)

This program grows from program 1 to let CPX respond to the light level measured differently depends on whether if it lies within or outside the “constrain” I set for “limited light”. The “if” statement can be a little confusing since it sets a relationship between 2 interrelating variables “light” and “limited light”. However, it simply means that I ask the CPX to measure “light” which is the environment’s light intensity and compare it to the range of 100~200 that I set for “limited light”. If light level lies within that range, then all pixels will turn green, otherwise all pixels will turn white.

(Important side note here: the position of “light” and “limited light” doesn’t matter. Because either block will end up measuring the same input which is light intensity. As long as there is a logical correlation established between the two, the CPX will read the light intensity and comparing it to the set range for “limited light” and respond accordingly).

## **Program 3: Actually useful program monitoring the range of temperature of freezer**

[https://makecode.com/_18JUmw0yhi9q](https://makecode.com/_18JUmw0yhi9q)

This program is a similar one to program two but it is actually useful in daily life. I used it to measure another input which is temperature. I first set a variable “temperature” which varies with the temperature detected by the CPX. Then I set a range of -4~4 ºC for a new variable “freezer temperature” using “constrain” which corresponds to the range of temperature I want my freezer to be at. Using the same logic “if…then…” statement to see if the “temperature” lies within the range of “freezer temperature”. If the temperature lies within the range, all pixels turn green and signals normal function of freezing. If not, the sound “siren” will be played and all pixels will turn red to double-alert someone to check it out. I also added another block to stop all the sound if button A is clicked. That is to prevent the people fixing the freezer gets too irritated by the sound (which could be probably after 5 seconds) and smash the CPX.
