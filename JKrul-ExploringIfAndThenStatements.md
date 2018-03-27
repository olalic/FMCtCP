# Chapter 2

## Exploring If and Then Statements

MakeCode, courtesy of Microsoft, is a simplified version of computer programming that makes learning to code basic concepts easier to grasp. I recently took an interest in exploring “if and then” statements. Explicitly explained, an “if and then” statement is used in computer programming to perform tasks based on a given condition. The “if” part of the statement is the given condition and the “then” part of the statement is what the program does. For example, “if the temperature is less than 32 degrees Fahrenheit, then wear a winter coat,” the ‘if’ is the temperature being less than 32 degrees (condition) and the ‘then’ is to wear a winter coat (what the program does).

![pexels-photo-54206.jpeg](https://josiahkrul.files.wordpress.com/2018/03/pexels-photo-54206.jpeg?w=1100)

To explore “if and then” statements, I started out with a very basic condition and action. The condition was the onset of a loud sound, so if a loud sound was registered, then the CPx would flash red. Then I made another statement that said if little or no sound was registered, then the CPx would flash green. Being that I made the code in a library, I had the idea that if the library was too loud, the CPx would flash red to show that it’s bad to be loud in the library. If the light was green, then the amount of noise being made is acceptable for the library.

[https://makecode.com/_VfxUsXU8fcHu](https://makecode.com/_VfxUsXU8fcHu)

[https://www.useloom.com/share/177fdf8984d449278e009e7001f4ef29](https://www.useloom.com/share/71253a46eb4e4581a42e708a778962a4)

To develop a more complex program using “if and then” statements, I wanted to see what would happen if I put an “if and then” statement within another. I added the term “else” to the “if and then” statements in my code, which means that if the condition is not met, then do a different action. In the example of the winter coat, “if the temperature is less than 32 degrees Fahrenheit, then wear a winter coat, else, don’t wear a winter coat.” Based on this code, if the temperature is 70 degrees, you wouldn’t wear a winter coat.

To put else statements into practice, I created a code for a nightlight. What I ultimately ended up doing is embedding multiple new “if and then” statements into the else section of the previous “if and then” statement. What I mean by this is I would add another “if and then” statement for the program to read if the condition in the first statement was not met. Eventually, I made a few “if and then” statements to cover any possible brightness that can be registered by the CPx. I set the code to increase the brightness of the LEDs on the CPx as the registered light input read by the light sensor on the CPx was lower. This way, I was able to accurately resemble what I would want a nightlight to do.

[https://makecode.com/_8A15ee386VDe](https://makecode.com/_8A15ee386VDe)

[https://www.useloom.com/share/177fdf8984d449278e009e7001f4ef29](https://www.useloom.com/share/177fdf8984d449278e009e7001f4ef29)

From a different perspective, I tried to see how many different “if and then” statements I could make to see if it would noticeably affect the speed at which the program would run. I also wanted to see how the preprogrammed “dark” function works in makecode. What I found was that my more complex program functioned at a rate too fast to noticeably see a difference. The “dark” function in makecode made reading the code significantly easier to read, however, I wasn’t able to completely recreate the complexity as I was able to do by embedding many “if and then” statements.

Basically, my programs are reading the light level through the sensor on CPx and representing the light level as a decimal. The more light read by the CPx, the higher the numerical representation of the brightness will be. As a reflection of the changing light level, my program creates a brighter light on the CPx at the sign of less light in the surroundings.
