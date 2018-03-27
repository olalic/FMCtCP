# Lucy Does Conditionals & Loops

Hi! I'm Lucy Faust! I'm excited to show you what I've learned in MakeCode this year using loops and Boolean functions in this semesters edition of LucyDoesDCS.


# Boolean Functions



Here is the transcript for my video which is embedded above:
Today I will be explaining a question posed by our class as a whole. The questions was “What is a boolean function and how can we use them in code?” To answer it, I will first turn back to what we discussed in class back in January. We discussed the idea that boolean functions are systems of statements where something is either true or false and follow under a big category of conditionals.

  

This first program is my simplest program to understand boolean variables. For a simple background, sound decibels range from 0 to 255. As you can see I have programmed this CPX so that if sound level is above zero, that is to say that it is true that there is sound, the CPX will be red.

  

To go a step further, this next program highlights both the true and false elements of a boolean function. This program is on a forever loop where if the sound level is above zero AND the sound level is below 127 decibels, the halfway point of measured sound on this program, then the pixels will be set to red. If this criteria is not true, that is to say that the sound is at a medium volume or louded, then the CPX will set its pixels to blue. What is important to note about this program and the elements of the boolean is that even if sound is above zero, the first condition on this program, the and signifies that the other conditional must be true as well for the pixels to set to red. To highlight the power of boolean functions and this phenomena further, we constructed a truth table as a class which can help solidify this idea as well.

  

My third program, the one that essentially does the exact same thing that the first one did but it is reworked because it the program does what the first program does but the program is written in a different way. Even though the conditionals are written differently, since they have the same requirements, the CPX runs the same. This program will set pixels to red if sound level is above 0 or of sound level is less than 255 (which is the max decibels anyway) so they produce the same red. Notice, in this specific case, regardless if I use the AND or the OR conditional, the CPX will turn red with any sound.
