# Loops in Makecode and Python #

## What is repetition how does it interact with a loop? ##
The goal of this exercise is to introduce a fundamental understanding of the function of loops in Makecode. When thinking of Makecode and connecting it to in python, one can view the similarities between the loop. In this post, I developed various programs that illustrate what repetition of the loop is and how it is used in Makecode, which I later translate into Python. The first program is the most basic, and the second and third become more elaborate. The final section of this chapter takes the third program and translates it into Python. 

## The first program: ##
In the first program, I used a forever loop. In the forever loop, I specifically used the “set all pixels block” to red for ½ a second and then to blue for ½ a second. This caused the light on the CPx to change colors. Specifically, the CPx stays red and blue for ½ a second because the block was positioned to change color for that specific time. It is important to note that when using the forever loop, the CPX will continue to repeat this pattern forever or until stopped. 


## The second program: ##
In the second program I made the loop more complex. Still using the loop forever block, I inserted the logic block (the “if then” statement) to add to the forever loop. Stating if button a was pressed then all pixels change to red for ½ a second and change to blue for one second. The if then statement then declares if button b was pressed then all the pixels change to red for one second while the CPx pixels change to blue for ½ a second. 


## The third program: ##
In the third program I added yet another logic statement, “else if” stating that if buttons A+B are pressed then it resets and goes back to the original settings where the pixels turn red for ½ a second and then turn blue for ½ a second. 

## Translation: ##
There are various steps to translate Makecode programs into Python. In this section of the chapter, I will take the third program (as shown above) and explain the steps I took to translate it from Makecode to Python. 

The first step when translating Makecode into Python is inserting “from dcs import *.” This library enables me to program the CPx through Python instead of Makecode, as well as containing the shorthand for the functions that will program the CPx. Once, I inserted “from dcs import *” it is easy to convert the functions from Python to Makecode because they are very similar. As shown below, in Python, the forever loop in Makecode is translated as “while True.”  In Python “If” still embodies the same function as the “else if” statement in Makecode. Also, “set all pixels to” is also the same in Python. In Python “sleep” is the same as “pause” in the Makecode programs. Thus, the only extra code I had to add while translating it over into Python from Makecoe was “from dcs import *.” 

