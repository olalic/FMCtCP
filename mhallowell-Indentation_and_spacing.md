##          Indentation *and*  S p a c i n g
This chapter focuses on making indentation and spacing clear using if-statements and while-loops.

For the first program, I made the simplest code I could think of that involved indentation. Its only job was to turn the cpx red forever. In Python, there isn’t a direct “forever” loop, but a while-loop is equivalent. The indentation is clearer in Python, but both programs show that the performance function is inside of the loop. If “setAllPixelsTo(RED)” wasn’t indented, the program wouldn’t run. An error may occur saying “expected indentation,” which is required in order for the program to work.

https://makecode.com/_9DKixdLKf65V

![Screen Shot 2018-03-13 at 8.44.14 AM.png](https://lh6.googleusercontent.com/MRob3W86c6E-njEcqlsZXQuO2RXiGci4hgGy_5SJTUnoqhA_AoXUEYzEm81i-r5tNKp83VRTyLXdGbPafFJC_86JEK2uctmciR6jmjl0uRuum8tNTaVBHaZfA-3gKgHKcNTi_pSb)![Screen Shot 2018-03-13 at 8.58.49 AM.png](https://lh3.googleusercontent.com/zyFDYlvaxDATXkgdM2ywS7r0pxiHP2XzUrWWtmJOkSvu6-Ld_rlELEBtcjextnKTZN26L8fHSH0qmQe7slUFGaVrOa2tijF_4dH0N0zjzzdJJxLgLF7dYO9quBTicDXVV4jMkRT3)
____
The next program I wrote was slightly more complex. It adds another layer or two of indentation to show the importance of it. When I take “setAllPixelsTo(GREEN)” and move it into the while-loop and outside of the if-statement, the program gets conflicted with multiple true statements happening at the same time. It then tries to perform both functions at once, flashing between the two. I explain this in greater detail in my video.

![Screen Shot 2018-03-13 at 8.45.02 AM.png](https://lh4.googleusercontent.com/6WpicTm2hUQvmvo4LAfacT9LVqWg4BoNt9WfZOM6kZNW9PO11FosSjQksFRYtR0HD_gBudEoViUJRfHtvXcMYiXhCcx5dIVsoLFJSuW89ppsT9JwaVOVFVyVeYCjAtDRrTGvEdKW)
![Screen Shot 2018-03-13 at 9.14.56 AM copy](https://lh6.googleusercontent.com/BX4m0wx9t-50yG6X1EXih8FzW8B-9Q1cmHP9VuF3qalCi2NU7Ixtt-IVsTKvIb36p7gOU0B1923tjRG4YidSYdYxpMdgWGZZtHGAxSjtZ45W8fO3wLegfyXQ1ZWrk4-5AyNOKkB6)
____
As is true in coding, there are multiple ways of creating the same code. The last program is another way of creating the second program I made. It involves less indentation, and it is therefore, in many ways, simpler. Everything is encapsulated in the if-statements. Additionally, I mentioned spaces towards the end of my video. Spaces are important in variable naming, because you cannot have spaces in variable naming. If things have a type of separation, then spaces do not matter. I could put any amount of spaces between a function and the arguments and Python would ignore the spaces and run the program properly.

![Screen Shot 2018-03-13 at 9.15.27 AM.png](https://lh6.googleusercontent.com/4CS0wF7tW5BuDLYURlc0L-KdZC_Eha-ddei5V-DgpNLv2UdQg5Cxm12NoIDWdVqnUfV5agZ2PMq3D2VnOGIJhVHSxuShVLQYjIpq6Hhosb_WeIYM7EMNqdjeUEiHxd9ot4l5INWp)

while True:

	if getLux() > 0 and getLux() < 155:
	
		getLux() > 25 and getLux() < 45:
		
	elif
			setAllPixelsTo(RED)
			
	else:
			setAllPixelsTo(GREEN)
			
		setAllPixelsToRGB(0,0,0)

![screen-shot-2018-03-13-at-9-14-56-am-copy3.png](https://lh3.googleusercontent.com/2wd4T2LAkGGsGvKme3emsHvyvxdpi24yKj7WXWJT5kgz-XIN5ze68_GFhFXrj0JfJjJfB4z3DrtdeBgEkoNBEzR3WAoE8Nvve-mbcImAVK4nZckuh-Ip-vU6FQfvvuouBd1aeoRQ)
____
