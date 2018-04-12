# Classes and Object Instantiation 
### What is a class?
A *class* can be understood first as a user or programmer defined type. While types like integers, float point numbers and strings are built into Python (and other programming languages), classes let the user define their own types. Just as we can create a specific member of one of these primitive types, we can *instantiate* a class as an object. A class can be thought of as a factory for objects. Every time one calls a class and assigns it to a variable, that object instantiation can do everything that is specified in the class.  
### An example.
I began with a simple example for classes by creating a class called "Point." To do so, all I did was write "class Point:". This syntax tells Python that everything after this line will be in the class called Point.

Next I began to program some functions for this new class. First I defined a way to assign values to the x and y coordinates for the point that I will instantiate. Next I created a function that would find the distance between them. Last, I designed a function called "main()". This is where it gets a little complicated. 

Because Python thinks that the rest of file after "class Point:" is in the Point class then there is no way to call it as an object without first leaving the class. One way to do this is to create a function in which you instantiate all of the object and then run that function. This is why we need the last two lines: "if __name__ == '__main__': main()". These lines tell Python that if there is a function named '__main__' then it will run the main() function that is in our Point class.
### Video.
[Check out the video.](https://www.useloom.com/share/0719ed16604c48338156417aa2fee675)
