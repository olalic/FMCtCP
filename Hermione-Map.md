# “Map” Block Exploration

Recalled how painful it was to use 5 consecutive “if” statement to match the brightness of pixels with a range of light level detected, I figured it would be a good idea to use a mathematical function linking the magnitude of input with that of the output. The block can function like that is "Map".

**Program #1: Just Map**

[https://makecode.com/_gvWUy97VL7CC](https://makecode.com/_gvWUy97VL7CC)

<div style="position:relative;height:calc(300px + 5em);width:100%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.adafruit.com/---codeembed#pub:_bspCj6WMRHyg" allowfullscreen="allowfullscreen" frameborder="0" sandbox="allow-scripts allow-same-origin"></iframe></div>

The function of block "map" is to translate any number within the a range "from x to y" to a number in the new range "from x1 to y1" proportionally. This program uses “map” to translate input “light level” which has a range of 0~255 to  0~10 . The first block on map is the variable being measured, which in this case is the "light level". Below it is the input range we want to translate: “0″ & “255”. The last two blocks are the corresponding range I want “0” & “10”. This piece of the program simply translates any light intensity detected by CPX to a number lies within 0~10 range proportionally. So, if I get input “200”, the output value should be 200/255*10/1 which is 7.8.

**Program 2: Automatically-Adjusted-Light, Finally**

[https://makecode.com/_9mpaJrE6oMKq](https://makecode.com/_9mpaJrE6oMKq)

This program is to use the simple block "map" to let CPX read input light level and give an output light level whose intensity corresponds to the input intensity. Continuing on the numerical relationships established in program 1. The output range 0~10 corresponds to the number of pixels on CPX. The output number is defined as "light-to-pixel". Then use the "for index" block to constantly commanding the CPX to measure the output number from the map. The number will be the number of pixels lit up in red under this block. However, if I want the number of pixels lit up to be inversely proportional to the light intensity, so that it actually functions as a flashlight in dark spaces and conserves energy in light spaces. I switch the range from 10~0. In this way, the darker the light intensity detected, the brighter it will be because more pixels will be lit up.

Videoes (apparently I wrongly pressed “stop” twice when I meant pause, so here are 3 videoes for the same topic):

[https://www.useloom.com/share/1ef78bbfbf274fcb94f69864016ef440](https://www.useloom.com/share/1ef78bbfbf274fcb94f69864016ef440)

[https://www.useloom.com/share/3b78dcc13a414830b599ebdd8d05e50d](https://www.useloom.com/share/3b78dcc13a414830b599ebdd8d05e50d)

[https://www.useloom.com/share/ec3c97f0e7e747499486e8ea3a6ca7a2](https://www.useloom.com/share/ec3c97f0e7e747499486e8ea3a6ca7a2)

**Program 3: The Fridge Guardian**

[https://makecode.com/_h45i5688yffq](https://makecode.com/_h45i5688yffq)

This program makes the CPX more sensitive to the input temperature by setting a greater output range and then the output decides what the CPX does to indicate the environment's (in this case a fridge's) temperature . The temperature's input range is amplified from “-5~45” to “0~100”. Hopefully, the sensitivity of the temperature sensor can allow this translation to be useful: it basically makes the temperature measurement to be more accurate to reflect a 0.5ºC change rather than 1ºC. Then I define an acceptable range I want to be 0~5ºC which translates into 10~20 in the output range. Within that range, the green lights will be on to show that the fridge is working properly, otherwise, it shows red light as a warning. Ideally, putting CPX into the fridge, it can tell you if it’s working properly to maintain the ideal range temperature. 
