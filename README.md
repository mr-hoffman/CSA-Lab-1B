# CSA-Lab-1B

## MyShape
Write a program that calculates and displays the perimeter and area of a rectangle using double amounts for the length and width provided by the user.
* In the `main` method, declare appropriate variables for length, width, and the rectangle’s area (do not initialize them).  Create a scanner object, and prompt the user to enter values for length and width, storing those values into the appropriate variables.
* Write a method outside of `main` to calculate the perimeter (this is still within the class, so it should be after the `}` for main, but before the `}` to end the whole program).  This should be a static method that receives length and width as parameters and does not return any value.  This method should calculate and print the perimeter of the rectangle (make sure to add words to the print statement so the output shows that the value represents the perimeter).
* Back in `main`, call the perimeter method, sending in the appropriate variables (since the method and main are in the same class, you do not need to use dot notation but rather make the call with only the method name).
* Test what you have so far to make sure the perimeter is calculating and printing correctly.
* Below the perimeter method (but before the `}` that ends the class), write a method to calculate the area of the rectangle (make sure your method name is not the same as your variable name).  This should be a static method that returns the value of the area and receives length and width as parameters.  This method should not have any print statement, but rather has a return statement.
* Back in `main`, call the area method, sending in the appropriate variables, and store the result of the call into your area variable.  Still in `main`, print the area of the rectangle (make sure to add words to the print statement so the output shows that the value represents the area).  
* Test your program to make sure both area and perimeter are calculating and printing correctly.

## RoundThings
Write a Java program that calculates and displays the area and circumference of a circle and the volume and surface area of a sphere.  You will be writing two classes for this program.  One will use the `RoundThingsDriver` class and the other will use the `RoundThings` class.

### ClassName
`RoundThings` - There will not be a main method in this class. It should go below the `}` that ends the `RoundThingsDriver` class. Do not put the word `public` in the class name declaration. This class will just have four methods.

### Methods
All these methods will be static. Use `Math.PI` for pi. the radius parameter will be a `double` value.

`calcAreaCircle()` - receives the radius of a circle, and returns the area
`caldCircumCircle()` - receives the radius of a circle and returns the circumference
`calcAreaSphere()` - receives the radius of a sphere and returns the area
`calcVolumeSphere()` - receives the radius of a sphere and returns the volume (watch out for integer division)

### ClassName
`roundThingsDriver` - This will have the main method and will call on methods from `RoundThings`

#### Input Variables
`radius` - a double value taken from a `Scanner`

#### Other Variables
These are to be calculated in `RoundThings`
`area` - a double
`circumference` - a double
`surfaceArea` - a double
`volume` - a double

### Processing
In `main()`, declare all variables listed above and create a `Scanner` object.  Prompt the user to enter a value for the radius and store that value into the appropriate variable.  Call the methods you wrote in `RoundThings` and store the results into the appropriate variables (since these are static methods, the call will start with the name of the class where the methods are written). 

### Method
`outPut` - this static method should be below the main method, and will receive 4 values as parameters:  a description of the type of value calculated (i.e. circumference, area, volume, surface area), one for the shape name (i.e. circle or sphere), one for the radius inputted by the user, and one for the actual value calculated.  It will not return anything, but rather will display (print) the information formatted nicely (see below).

Ex:   	
The **area** of a **circle** with a radius of **#** is **#**.		(**# will be replaced by the
The **volume** of a **sphere** with a radius of **#** is **#**.  appropriate value.)

### Processing
In `main`, call the `outPut` method four times.  The first time should be for the area of a circle.  The second time should be for the circumference of a circle.  The third time should be for the surface area of a sphere.  The fourth time should be for the volume of a sphere.  They should all use the same radius value.


 ## StringProgram
Write a program that reads in a single `String` from the user containing exactly four words separated by * symbols with no spaces into a single String object. Next, extract each word from the original string and store each word in a String object. Then concatenate the words in reverse order to form another string.  Display both the original and final strings. Hint: to extract the words, you should use the `indexOf()` method to find each symbol * and then use the `substring()` method to get the characters between the * symbols.
Example output:
```
Original:  one*two*three*four
Reverse:  four three two one
```



