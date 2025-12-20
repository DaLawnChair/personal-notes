

Reference:
https://www.youtube.com/watch?v=tD5NrevFtbU
* Using the example of calculating the area of a given shape, we see massive improvements from avoiding the simple principle of clean code in the space of C++
* Clean code guidelines:
	* Polymorphism
	* Do not use if/switch statements
	* Keep everything virtual, do not let things be internal
	* Keep functions small 
	* Let functions do 1 thing
	* Do Not Repeat Yourself with same instances of code
* During the video he outlines how slow these things are in the given order
	* Polymorphism: 35 cycles per shape
		* as the values are stored as objects of different properties (ie circle will have the pi constant along with a radius, but a square will just have its side length, thus in a list it we must have pointers rather than the object itself and must be dereferenced)
	* Do not use if/switch statements:  24 cycles per shape (1.5x)
		* Use a switch for the area calculation based on an enum denoting the shape_type and a fixed class size for width and height rather than calling each object's area() function and having each one contain certain properties
		* No more overhead from having classes to and calls to the function callstack
		* no need to call off of a pointer 
			* compiler is able to optimize the code as it won't have to guess what kinds of types might be derived from the base class
	* No internals, functions are allowed to know what the object is. ~3-4 cycles. (10x)
		* replace switch statement for shape  with a simple calculation of a coefficient\*width\*height where coefficient is defined for each shape type
		* note that doing the switch statement case, this relationship is easily identifiable where in polymophism the property is nested between classes and (likely) file
	*  Using a different method now, of calculating the relationship between area/ (1+corners of the shape)
		* polymorphism example has the function cornerCount() and Area()
			* due to the rules of clean code, we should keep these functions seperate
		* the if/switch example uses switch statements to get the corner count. same example as before
		* the no internals case fuses this as coefficients.
		* findings: 
			* polymorphism: 43.87
			* no if/switch: 23 (2x)
			* no internals: 3.5 (15x)
* these are crazy findings for a small case, without any actual optimization from usage of memory/cache localization or CPU tricks 
	* Using lightly optimized AVX:
		* Up to 24x
* Summary:
	* do not use OOP for trivial calculations that can be easier to implement with simplier concepts,. or else you will deal with a lot of overhead and headaches in performance
	* Here is a sample of the code from a [reddit user](https://www.reddit.com/r/cpp/comments/11gnpvv/comment/japdre7/?utm_source=share&utm_medium=web3x&utm_name=web3xcss&utm_term=1&utm_content=share_button):
	* https://pastebin.com/raw/CYzCYSer