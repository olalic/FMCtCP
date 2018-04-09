# Introducing Arrays in Makecode
For my second video, I decided to investigate arrays. It turns out that Python actually doesn’t have a specific array function; instead, it has a more general “list” function which can be used to do the same thing as an array. However, I think it’s important that we take a step back and investigate arrays in Makecode, since we may never have gotten comfortable with them. This is a basic array:

![Screen Shot 2018-03-18 at 6.59.00 PM](https://lh4.googleusercontent.com/rBgyHLFvLrrxj79hmncPvtUix-saLUf9wW3jlpdMNxHdpp66xrhiOR8hlNR-peUucE2sDF4bL5iZfTpFSaG1-e3XmBovBMHKoGcdiMsATfBg7le32B9oolUdlJR3psc8BFUVaDGp)

The three necessary parts of an array in Makecode are 1) define a variable as an array and fill in the values you want the array to store. 2) Create a loop that determines how to run the array. Our array has 6 values starting at 0, so we need to tell the array to run the array from 0-5, hence the length of the list (6) minus 1 = 0-5. 3) Finally, inside the loop determining how to run the array, we need to run the array. So just like other programs, you need to define a variable, create a loop for that variable, and perform an action on that variable.

This next program runs the array, and then runs the array in reverse is light level is below 128. What I learned from this program is that no matter what you do to the array (i.e. tell it to reverse its order), you still need to give it a loop and command, or it won’t output anything. Arrays are simply stored data. They won’t perform any action unless you tell them to.

![Screen Shot 2018-03-20 at 7.54.11 AM.png](https://lh4.googleusercontent.com/rLZ9kMT8WBV6o-lwqi0eRMX6ayOEyAUKe5_mgSy8dMYKxlyVnnDV9f6_0I8t8lURSH_vqJBcCyTcQAsjnwO530CmbOKy3VyuL5YOWHYjfobidJHlXaxyAevocxoNAij1KWICT_6C)

My third program is very similar, except that the reverse instructions are embedded in the first array loop. This allows me to change the direction in the middle of the array by manipulating the light level. It prepares to run the array, checks the light level, and then then decides which direction to run. If light level is 128 or above, it will skip everything in the while loop and run the forward program. If light level is below 128, it will stay within that while loop, so there is an implied “else” outside the while loop. Something to note is that the program will reverse the direction of the array each time it runs, so you will get an alternating pattern.

![Screen Shot 2018-03-20 at 8.11.34 AM.png](https://lh5.googleusercontent.com/xkjL8XFsxVPs_pdvvR4B2Lxwvis5OInBt0nJPC6W1sXBte4x1jZKi-G4ZQ3pdQ4stUTL18pgC5Bwk5haBKFYzRABbWwgBAFBiTWl61JOJ4ZJD-2f8Y_k8Kqa5cnOP_bgWPxfV5GE)

[Link to my video on arrays](https://www.useloom.com/share/beeb80c0bb6649ce9244b936ffaeb431)
