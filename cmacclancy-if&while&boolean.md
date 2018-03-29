
## Whats the Difference Between if and While Statements?

- ***If statements*** are the simplest form of conditional statements, statements that allow us to check conditions and change behavior/output accordingly. The part of the statement following the if is called the condition. If the condition is true, the instruction in the statement runs. If the condition is not true, it does not. The *if statements* are also *compound statements*. They have a header (if x) followed by an indented statement (an instruction to be followed is x is true). There is no limit to the number of these indented statements, but there must be at least one.
	* There is a second and slightly more complicated layer that one can add to if statements: **alternative execution**. In this case, there are two possible outcomes. In this situation, the condition determines which outcome runs. For example, If x>=0, print (‘x is positive’) else: print( ‘x is negative’). These alternatives are known as branches, as they are “branches in the flow of execution.”

- ***While statements*** determine whether a statement is true or false. If what’s stated is true, then the program runs the statement and returns to the first step. If what’s stated is false, the program exits the while and goes to the next statement.
	* An added step to while statements is turning them into continuous loops. If you don’t change the value so that the condition is never false, the while statement becomes an infinite loop.

**Makecode:** There are also ways to format these statements with the blocks on makecode. For the if statements, you can select the Logic “if/ then statement” and fill in the blocks with your desired conditions and outputs. For example : “if x>0, set all lights to red.” You can also easily format the forever “while” loop in makecode, using the Loops block “forever.” Then, “if x>0, set all lights to red.”

Below is a link to a walk-through tutorial/ demonstrations of the material described above:

*The video is slightly redundant when explaining make code- whereas in the video the If statement is demonstrated using the forever loop, it may have also been accomplished using the “on start” loop.*


https://www.useloom.com/embed/0961ef11174f483ea0ece5ba4544b399

------


##  What is a Boolean Expression?

A **Boolean expression** only has two possible values: *it is true, or it is false*. In its most simple sense, you can make a Boolean expression on make code using the blocks. Under the “Logic” heading, there is a “Boolean” subheading which contains “true” and “false” blocks. These can then be used to plug into any place a boolean value is expected.

When working with Boolean expressions, you can also use relational and logical operators. Relational operators compare the operands using =, <,>, >=, etc. Logical operators combine boolean expressions using “and”, “or”, and “not”. The relational operators can be found under the logic heading on makecode, under the subheading comparison. The “\_\_and\_\_”, “\_\_\_or\_\_\_”, and “not___” can also be found under the logic heading, under the subheading “Boolean.”

You can also use relational and logical operators in python, though in python they look a little different. When using relational operators, “==” is equal to, “!=” is not equal to, and “>, <, >=,” and “<=” are all as expected. For example, the operator “==” compares the operands to determine if they are equal (true) or unequal (false). An example of conditional operators in python would be “3 == 3 and 2 == 2.” AND dictates that BOTH must be true in order to be true and thus we would expect the output “true”. If one was not true, we would expect the output “false.” For another example we could use the logical operator “or.” If “4 > 2 or 1 > 2”, OR dictates that EITHER one or the other must be true, so in the case because the first operand is true, we would expect true.

A video demonstrating these concepts can be found below:

<iframe width="630" height="394" src="https://www.useloom.com/share/2493e4b0afb04a07a55cc2e3d1f03bde" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>

https://www.useloom.com/embed/2493e4b0afb04a07a55cc2e3d1f03bde
