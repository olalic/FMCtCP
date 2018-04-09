# 3 PROGRAMS THAT EXPLORE BASIC PYTHON SYNTAX AND VARIABLES

My DCS class is exploring basic python, so I wanted to share 3 programs that feature basic parts of the language.

## Program 1
  The first program simply demonstrates the output of strings and variable values into the command window.
  
  In line 1, we print the string “Hello, let’s explore variable types.”
  
  In line 2, it assigns a variable, eq, to the value of the mathematical equation: 3^3 + 5/6 + 4.1 +2.2.

This program demonstrates some of the mathematical operations that python can compute. It also shows a few of the types present in python such as integers ( numbers like 1,2,3…), strings (‘insert characters here’), and floats (numbers like 1.2, 3.7, etc).     

It ends by showing that the print command can be also be used to output the values of variables to the command line.

> #Simple program  
> print(“Hello, let’s explore variable types”)  
> eq = 3\*\*3 + 5/6 + 4.1 \* 2.2  
> print(eq)

## Program 2
My second is slightly more complex. It builds on the ideas of first one to show that mathematical operations can be accomplished using variables.

I have two variables (eq and eq3) that rely on the values of previous variables.

It is also demonstrated in this program that print statements can be used to provide context to outputs in the command line.

Next, we will build further on the concept of doing math and how to use variables in the final program.

> #Slightly more complex
> 
> eq2 = 1/eq  
> eq3 = eq + eq2
> 
> print(‘eq3 relies on eq and eq2’)  
> print(eq3)
## Program 3

My third program demonstrates usage of while loops, variables as indexes, and how comments can be used to provide useful information to the reader. I wanted to create a variable through addition in a new way.

First, we index our while loop with the variable n and assign it the value 0. We also assign our variable eq4 its value.

While n < 3, our loop runs.

The loop first adds eq4 to itself (using the += operator) and then increments the index by 1. Since n=0 and we add 1 to n during each iteration of the while loop, we ensure the loop runs 3 times.

Each loop, we also print n and eq 4 so we can check the loop is running correctly. Print commands are valuable in debugging as we can make sure that operations are being computed corrently and in the correct order.

Overall, this program demonstrates how print statements can be used to help illuminate what your computer is really doing when a script is run.

> #Complex done a different way  
> n=0 #n indexes the while loop  
> eq4= eq3 * 1.5  
> print(eq4)  
> while (n < 3):  
> eq4 +=eq4 #add eq 4 to itself  
> n=n+1 #increment our index  
> print(n)  
> print(eq4)

Here is a  [link](https://youtu.be/VCrjBq6B-IA) to my guided explanation of these programs.
