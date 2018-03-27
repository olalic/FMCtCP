# Investigating Spacing and Indentation in Python

For the previous assignment, my group investigated spaces and indentation formatting. We decided that this topic might be too narrow for this assignment, so we all explored different topics individually. I decided to expand my topic to the role of grammar in naming variables and conditional statements. This first program simply initializes the variable acceleration in the z axis without using it yet, and sets all pixels to red as long as true is true (forever).

![Screen Shot 2018-03-12 at 11.27.31 PM.png](https://lh3.googleusercontent.com/GnR1zbfAP-JeZWzMvdLQQeKBAELnAwE1QdSnsGGkMLbxMnPRF4lYirIwyxe5Xn3jRRULjRMbgP8psUb2RUElsMn2WPGJnd2jP2gzmNUhDw39wc8Zhqbx0VJ8zF1sr7mXLB5XPVnJ)

![Screen Shot 2018-03-13 at 8.08.54 AM.png](https://lh6.googleusercontent.com/qu2a2UD8mEk0KE-73IWY00xJa6qfMKZsbWIqM_QkzPfrKK2_UyaBjZZDKyjngYO54UZAmBJaOAgSg7BD_NcC1Cx0IeqE4e8eR-Zkc0BDj1ASk-EDfBKfonbyrhHYOL32Z_596HTR)

For my more complex program, I introduced a conditional statement. Still defining the acceleration as accel_reading, I also set it equal to zero on start. I’m not sure if that’s necessary, but it’s in the Rosetta Stone. Then, I wrote my if statement, followed by a colon, which automatically indented the next line 4 spaces. Using the setAllPixelsToRGB command, I made the pixels yellow when the CPx faces down and blue when it faces up.

![Screen Shot 2018-03-12 at 11.44.43 PM.png](https://lh6.googleusercontent.com/Pp8gMwcbqiyot3lWbEBj47fjGKJHDnr3QCnUHE6edokkt60qZaeG-XAh1gKyXzFhZlXgvbFP5eL7A832krhJrii0WlI54syxRfPAv64WI8IacREuGXRyebWqDglKVnC1vZq453oF)

![Screen Shot 2018-03-13 at 8.12.40 AM.png](https://lh4.googleusercontent.com/KADMVrPePcn1eVxZgXxJLnuEgVupmX4UhUkyVOLioXlrEUBdBrsvz7BV_MoWUTxw_BLnbNDbSyVF5m1n93ufVzNbhmqMpRIix_gXIw6IXNM5-kuEetQUYzXJZQcyQntOEeK_oamm)

I brought in the element of spacing, which was the group’s original question, into my last program., which was the group’s original question. The program is the same as the last one, and would look the same in Makecode. The only difference is that instead of having putting a space before and after each value, they’re all values are crammed together. Although it doesn’t seem to change the output of the program, this code looks messy and is hard to read. From all of the python we have been exposed to, my brain registers the program above as the “standard” style. I also think this code would be harder to debug because there is no separation.

![Screen Shot 2018-03-12 at 11.46.20 PM.png](https://lh4.googleusercontent.com/kddKobyoStTlTXZRBI-uDQvDbp9DIJuiVS7TbPwJNu65hW2a4ntZagU1Hgq3oo9IjzG1u57k7WyMOs0qUi1g534HtkSfidTAYYacyMkUfExL1SpoE22e84HIjpK371yk2jVUQUJs)

[Link to my video on spacing](https://www.useloom.com/share/ab0910606bee4b6198cc04a5e9fd87e1)
# Introducing Arrays in Makecode
For my second video, I decided to investigate arrays. It turns out that Python actually doesn’t have a specific array function; instead, they have a more general “list” function which can be used to do the same thing as an array. However, I think it’s important that we take a step back and investigate arrays in Makecode, since we may never have gotten comfortable with them. This is a basic array:

![Screen Shot 2018-03-18 at 6.59.00 PM](https://lh4.googleusercontent.com/rBgyHLFvLrrxj79hmncPvtUix-saLUf9wW3jlpdMNxHdpp66xrhiOR8hlNR-peUucE2sDF4bL5iZfTpFSaG1-e3XmBovBMHKoGcdiMsATfBg7le32B9oolUdlJR3psc8BFUVaDGp)

The three necessary parts of an array in Makecode are 1) define a variable as an array and fill in the values you want the array to store. 2) Create a loop that determines how to run the array. Our array has 6 values starting at 0, so we need to tell the array to run the array from 0-5, hence the length of the list (6) minus 1 = 0-5. 3) Finally, inside the loop determining how to run the array, we need to run the array. So just like other programs, you need to define a variable, create a loop for that variable, and perform an action on that variable.

This next program runs the array, and then runs the array in reverse is light level is below 128. What I learned from this program is that no matter what you do to the array (i.e. tell it to reverse its order), you still need to give it a loop and command, or it won’t output anything. Arrays are simply stored data. They won’t perform any action unless you tell them to.

![Screen Shot 2018-03-20 at 7.54.11 AM.png](https://lh4.googleusercontent.com/rLZ9kMT8WBV6o-lwqi0eRMX6ayOEyAUKe5_mgSy8dMYKxlyVnnDV9f6_0I8t8lURSH_vqJBcCyTcQAsjnwO530CmbOKy3VyuL5YOWHYjfobidJHlXaxyAevocxoNAij1KWICT_6C)

My third program is very similar, except that the reverse instructions are embedded in the first array loop. This allows me to change the direction in the middle of the array by manipulating the light level. It prepares to run the array, checks the light level, and then then decides which direction to run. If light level is 128 or above, it will skip everything in the while loop and run the forward program. If light level is below 128, it will stay within that while loop, so there is an implied “else” outside the while loop. Something to note is that the program will reverse the direction of the array each time it runs, so you will get an alternating pattern.

![Screen Shot 2018-03-20 at 8.11.34 AM.png](https://lh5.googleusercontent.com/xkjL8XFsxVPs_pdvvR4B2Lxwvis5OInBt0nJPC6W1sXBte4x1jZKi-G4ZQ3pdQ4stUTL18pgC5Bwk5haBKFYzRABbWwgBAFBiTWl61JOJ4ZJD-2f8Y_k8Kqa5cnOP_bgWPxfV5GE)

[Link to my video on arrays](https://www.useloom.com/share/beeb80c0bb6649ce9244b936ffaeb431)
