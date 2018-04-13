
# Investigating Random Number Generators

Posted on  [March 20, 2018](https://pillaroftime.wordpress.com/2018/03/20/three-programs-three-paragraphs-part-2/) by  [pillaroftime](https://pillaroftime.wordpress.com/author/pillaroftime/)

**Coin Flip, Program 1:** My first program is meant to sort of recreate a coin flip. My goal was to explore the random number generator with this program and concept in mind. So in order to recreate the simplest coin flip in code I could find you first grab a ‘on button A,’ from the input section. Then drag an if, else logic under that, and replace the ‘true’ part in the if else logic with a comparison also in the logic section. From the math section drag a ‘pick random 0 to 10’ block and place that on the right side of the comparison. The symbol of comparison can either be less than or greater than it doesn’t really matter and on the right side choose half on the bounds for the random number that will be generated. Now under the if place a set all pixels to green and under the else place a set all pixels to red. The program should if done correctly, when you press the a button, have a 50% chance of lighting up green or red.

![2018-03-19](https://pillaroftime.files.wordpress.com/2018/03/2018-03-19-e1521514589683.png?w=1000)
---

**More Randomized Coin Flip, Program 2:** A bit more complex. This program is largely the same as the last one, I just wanted to utilize the random numbers a little more this time around. So under the the if, I placed a ‘set all pixels to black’ in order to just clear the lights on the CPX. Than set brightness totally because of personal preference really no other reason. Than a ‘set pixel color at 0 to (color),’ I dragged in a random number block from the math section and placed that over the 0 and changed the color to green. I did the same steps under the else but just for the color red instead. Now if done correctly, when the ‘a’ button is pressed a light in a random location should 50% of the time turn either green or red.

![2018-03-19 (1)](https://pillaroftime.files.wordpress.com/2018/03/2018-03-19-1-e1521516078270.png?w=1000)

---

**Alternatives, Program 3:** How to do it a little differently. I couldn’t really find another route which fundamentally changed the way in which I programmed it first. However just as I mentioned before the sign in the comparison logic can be either less than or greater than. The range in which the random number is picked can also be changed, you can also rig the game in this way. The colors green and red are arbitrary and so they can also be changed. Finally the button in which it is programmed to can be changed to another button, or even set on shake, or on a loud sound.

**Example Video:** 
<iframe width="630" height="355" src="https://www.useloom.com/embed/2e3316e2205e4b35bde7324990575164" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>


**Program 1 Coded in Python:** This is how the first program looks coded in Python.

![2018-04-13](https://pillaroftime.files.wordpress.com/2018/03/2018-04-13-e1523640113510.png)

**Program 2 Coded in Python:** This is how the second program looks coded in Python.

