# Chapter 2:

In chapter 2, we explore how the CPx reads acceleration along the Z and Y axis. To help, the chapter includes pictures of the command in MakeCode as a point of reference.

Let’s get started!

## Make Code:

To begin, we place a “set item to” block, found in the variables tab, within the “on start” block. In order to differentiate between the two axis, Y and Z, we must rename the “item” portion of this block to “accel_y_reading” as it will be used to read the acceleration along the Y axis. Similarly, we repeat the above step and rename the “item” portion to “accel_z_reading”.

**![](https://lh6.googleusercontent.com/oQGFd27xzXMw1fSd9annc6klVxow4x8o61o556AhQV0iMauWv_FETZU4qUL3TuCIdlWIrfEII82zg4YAnw6jL41MdhWsdm149NKqID74oMYwe8tcMGUDRo1mC0MkdEApg_gzE1oQ)**

Once we have the “on start” block complete, we move on to the “forever” block. It is here that we tell the CPx what we want to be done in specific situations. Seen below, this program tells the CPx to read the acceleration along the y axis. The CPx is then told that if there is an acceleration along the y axis, to set all pixels to red. Similarly, if there is no acceleration, it is told to set all pixels to green.

  

This step is then repeated using acceleration along the z axis where a recorded acceleration will turn the pixels blue and no acceleration will keep the pixels green.

**![](https://lh4.googleusercontent.com/XR-T-mcO3lbnVoXUczqwVecVu-NFjiaM3gg8nGjZVVs95JJcaOfgvpx_8eSlXQrIU1qFSlpH0RBMXipF7U2hmUt4qgZK9IJXhioiRiUkjnnoxC27cdRDH9axSxhg4QNMqLShqrKE)**

## Taking this to Python!

While I originally had trouble translating my programming in MakeCode to Python, the process became easier as I continued to spend time reading articles and watching tutorials on youtube. After a couple readings and 2 or 3 videos I was ready to go. Just as pictures from the MakeCode program were provided above, this section will provide screenshots of the Python code to serve as a point of reference.

Here we go!


To begin, we need to tell Python where we’re getting our commands from. To do so, we type, “from dcs import * ”. With this, Python understands where variables and commands are being stored. The inclusion of his line of code simplifies our translation immensely.

Just as our MakeCode program started with an “on start” command where variables were defined, we begin our Python program with defining our variables.

**![](https://lh3.googleusercontent.com/2_LSD1gQDT2e-XudPblmxwLA8Kcahl2Nut5O098emzmnq71-5EQXPcoGchiqt0lFXh1Q-QTe3Bz78QZTdvCrNMC3IeqnYSHdj28KhTlHRwEW3f67Aek95MifjW9YtJbHOFxOrMLX)**
 
 Moving forward, we look to begin coding our “Forever” block. In Python, this is designated with the code, “while True:” . Once these basic codes are established, we are ready to translate the code to Python. While this portion of the process may seem daunting, it is actually extremely similar to the process used in MakeCode.
 
 **![](https://lh6.googleusercontent.com/-BZdVbo_l3fYTONrPVmcZeNyplwvkr04pM3pZWw-L09d3Ebc7mYhnS_m7_v0Y3EpyAyOagecT_AE7aAl1oFf1S3ZWeG-VO2LRq16zfcqpw5w-EbONs80HJdjk23saKQCV1WB7lYY)**

