# “while” vs. “if” in Python
[**Screencast**](https://youtu.be/cwz9y7rYMHk)
## Program Set #1

[While Program](https://repl.it/@HanningXu/while1)

![enter image description here](https://gracehanningxu.files.wordpress.com/2018/03/screen-shot-2018-03-06-at-7-35-27-pm.png?w=740)

[If Program](https://repl.it/@HanningXu/if1)

![enter image description here](https://gracehanningxu.files.wordpress.com/2018/03/screen-shot-2018-03-06-at-7-36-30-pm.png?w=740)

Since I am exploring the differences between the “**while**” loop and an “*if*” statement, I decided to start my simplest set of programs with an addition command. Because I wanted to get into the nitty-gritty of how they are different, I kept both programs identical except for the **while** / *if* commands. Initially, I tried writing the programs using equal signs (so x = # instead of x < #), and both turned out to do the same things. However, when I changed to <, the differences between the two manifested. As you can see on the right side of the first program, the **while** loop did not stop running until the value of x was no longer smaller than 5. Meanwhile, the *if* statement only accounts for running through the indented portion once. To put it in another way, the **while** program is essentially running n  *if* statements (in this case, n = 5) one after the other, until x < 5.

## Program #2
[Game Program](https://repl.it/@HanningXu/Prog2)

Code when answer is correct:

![enter image description here](https://gracehanningxu.files.wordpress.com/2018/03/screen-shot-2018-03-07-at-8-34-08-pm.png?w=740)

Code when answer is incorrect:

![enter image description here](https://gracehanningxu.files.wordpress.com/2018/03/screen-shot-2018-03-07-at-8-34-54-pm.png?w=740)

Essentially, I wrote a simple program with two defined variables, a **while** loop, and an *if* statement, that imitates a game. In this game, if the player answers the question correctly (player\_answer = 1), he will be able to proceed to the next question; if he answers incorrectly (player\_answer = 0), it is “Game Over” for him. Because there are no signals feeding into this program, I am only considering the fundamental scenario of the player either getting all the questions correct (getting all 1s), or getting the very first question wrong (getting the first answer as 0). To stop the the **while** loop from running forever, I set the parameter for “points” to be between 1 and 10. As you can see in the first scenario, the **while** loop will keep running until the condition, 0 <= points < 10, is no longer true; so in this case, ten times around the loop. The *if* statement inside the **while** statement demonstrates two possibilities, and therefore two potential results to this game. If the player gets the correct answer, a value of 1 will be added to the variable “points”, and the loop will run again, until “points” is no longer between 0 and 10. If the player answers incorrectly, however, the program will print out the words, “Game Over”, and exit the program.

However, this short program would result in very different results if we take out the **while** loop. Sure, the program will still print out the words, “Game Over”, and exit the program if the player answers incorrectly. However, if he answers correctly, the program would only print out one value of “points” when we hit the run-program button, because it is only running the input through the *if* statement once.
## Program #3
[Finding Multiples Program](https://repl.it/@HanningXu/Prog3)

![enter image description here](https://gracehanningxu.files.wordpress.com/2018/03/screen-shot-2018-03-07-at-9-30-10-pm.png?w=740)

In this program, I told the program to print out a list of multiples of a between i and b, and specify whether each one of them was even or odd. This program has the same concept as my second program, just executed slightly differently. Similar to the last program, the **while** loop sets a parameter, so when the parameter is no longer true, the program ends. The *if* statement again separates the results into two categories: odd and even (if a\*x%2==0). If a\*x is even, the program prints its value and the word “Even”; if it is odd, the program prints its value and the word “Odd”. After the program does these things in the loop, the value of x increases by 1, and the program runs again (if the parameter is still true) or stops (if the parameter is no longer true).
