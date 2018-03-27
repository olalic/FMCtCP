# What Are Make-Code Blocks really?

The goal of this exercise is to further understand the structure of programs, functions, and libraries. When thinking of make-code through a python lens, I view many of the make-code blocks to be functions that have been defined by the developers. Essentially that is what I understand libraries to be. In this post I developed three programs on make-code; a very simple one, a slightly more complex one, and finally a third program that does what the second one did, but uses a function I defined instead of one of the blocks that make-code has already defined.

<iframe width="630" height="394" src="https://www.useloom.com/embed/584f5cd91f7446f0982205de1d86ae24" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>

**The first program:**  The sole purpose of this program is to set all pixels to green. Though it is extremely simple, there is more happening ‘behind the blocks.’ For instance, make-code knows what the “set all pixels to” block wants the CPX to do. This is because this function was previously defined and is called whenever I use the block. Similarly the block that is simply the color green, actually describes an RGB code: (0,255,0).

![Screen Shot 2018-03-12 at 7.40.35 PM](https://dcs102dot.files.wordpress.com/2018/03/screen-shot-2018-03-12-at-7-40-35-pm.png?w=248&h=279)

**The second program:**  This program is designed to change color when the sound level changes above a certain point. At first I defined the variable “Sound Level.” Then, in the forever loop the program sets all pixels to green if the sound level is below 2 and all pixels to yellow if the sound level is over or equal to 2.

![Screen Shot 2018-03-12 at 7.41.14 PM](https://dcs102dot.files.wordpress.com/2018/03/screen-shot-2018-03-12-at-7-41-14-pm.png?w=306&h=395)

**The third program:**  Finally, I use functions to re-create the pre-set blocks used in the second program. The two functions I defined are “set\_all\_lights\_to\_green” and “set\_all\_lights\_to\_yellow.” In each function, all ten pixels are told to turn green or yellow using a loop. Then in the forever loop I call the functions instead of using the “set all pixels to” block.

![Screen Shot 2018-03-12 at 7.41.23 PM](https://dcs102dot.files.wordpress.com/2018/03/screen-shot-2018-03-12-at-7-41-23-pm.png?w=425&h=299)
