Hi People. 

This is a brief tutorial on For Loops.

<iframe width="630" height="380" src="https://www.useloom.com/embed/3a16440dbf124a28a170a26bfb40bdb2" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>`


Repetition is good for computers because interpreting and following commands takes time. A computer needs a way to "loop" back over the same block of code again and again.

If I want a program to do something 100 times, rather than writing and running the same code, a for loop is more efficient than writing it in a 1000 times over and over.

For loops can come with conditionals (something that will not truly be covered in this tutorial, however, conditionals are good for telling a program to stop running.

How else would a program (computer) know when a code needs to stop "coding"? Computers execute tons of commands all the time, but they don't reason through them (unless you program that too).

For loops allow us to make some program do things until we give conditions that tell it to ~~STOP~~.


For loops typically follow this format: For all of the items/elements in a list, please perform ***some*** thing. In other words, do something.

Now we need an imaginary but soon-to-be-real list. So let's say we've got a list of shoe brands.

I've got some Nikes, Converses, Reeboks, and Adidas. Great. My favorites.


> **IN PYTHON, WE SAY:
> 
>  shoe_brands= ["Nike", "Converse", "Reebok", "Adidas"]**



This tells us, we have a list titled, "shoe_brands". The shoe brands on this list include: Nike, Converse, Reebok, and Adidas. Nice. These names are also referred to as strings.

Strings are characters that we can display, or, print. Quotation marks go around "string" variables. That is how we indicate that they are such.

Now let's put it in a for loop.


> **IN PYTHON, WE SAY:
> 
> for a_brand in shoe_brands:
> 
>  print (a_brand)



This says, for every item/element that is assigned the variable brands, in the list shoe_brands, print out the variable brands (that is, Nike, Converse, etc.).

This can be done with strings or numerical values. If we wanted to do numbers, we could do something like what you see below.


> **IN PYTHON, WE SAY:
> 
> evens= [2, 4, 6, 8, 10]
> 
> for a_number in evens:
> 
> print (a_number)


So, if we look at the REPL box (or whatever method you use for live coding), you can see the elements of each list appearing as the code is actually ran.

We see Nike, Converse, Reebok, and Adidas. Then we see 2, 4, 6, 8, and 10.



Let's switch over to the CPX and apply these same ideas to do some stuff.

The goal is to get some lights to do some things. So let's do some things.



***+Make sure you have the dcs import file (this contains some of the pixel/light commands we'll be working with).***

+You'll also need to use random import file for the last exercise. We'll discuss this more in a bit.


> **IN PYTHON, WE SAY:
> 
> from dcs import *
> 
> from random import *
> 
> for pixel in range(0,10):
> 
>  setPixelRGB(pixel, 220, 0, 220)

Each of these values– 220, 0, and 220, correspond to RGB settings for the CPX pixels. The range runs from 0 to 255 and you can choose any number within that range to produce a myriad of colors on the CPX.

The range(0,10) corresponds to each of the pixels on the CPX. There are ten of them.



*After running the code, you can see that each pixel –the circular bulbs–lights up with a bright Magenta color one by one.*

   <iframe width="560" height="315" src="https://www.youtube.com/embed/4s5Glg8g46M" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
    

If you want to go a little further, we can make use of the random function. This random function will generate and random number between 0 and 255.

Everytime this line of code is ran, the 10 colors that appear will change. Sometimes drastically, sometimes not, but the number generation is *~*at random*~*.

***If you would like to run the code below, make sure to comment out the code in line 46.***

   <iframe width="560" height="315" src="https://www.youtube.com/embed/LquLXgOGf1M" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
   
   <iframe width="560" height="315" src="https://www.youtube.com/embed/Gdl4gpj6wog" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

> **IN PYTHON, WE SAY:
> 
> setPixelRGB(pixel,randint(0,255),randint(0,255),randint(0,255))
> 
> pause(500)

This pause code line slows down the program to allow us to watch the lights move on the CPX.


