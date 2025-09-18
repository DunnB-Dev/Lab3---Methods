# CSCI 1250 – Methods Lab
## C# Static Methods

### Introduction
This lab will reinforce topics covered in the lectures about creating static methods, method headers, method bodies, return values, parameters, arguments, and variable scope.

---

### Part 0: Setup
1. Create a new C# console project, being sure to use “.NET” and not “.NET Framework”. The version of .NET used must be version 8.

---

### Part 1: Greeter
1.  Create a new `static void` method named `Greeter`. This method should accept no parameters.
2.  The method body of `Greeter` should display the following information to the screen:
    1.  An initialization message (such as ‘Starting Greeter method…’)
    2.  Your name
    3.  The name of this class
    4.  Your section number (ie, CSCI-1250-XXX)
3.  Inside of the `Main()` method of your program, call your `Greeter` method. Hint: Make sure to call your `Greeter` method inside your `Main()` method.
4.  Ensure that you were able to create and call the method before advancing.

---

### Part 2: Fahrenheit to Celsius Converter
1.  Continue the program from before.
2.  Create a new `static` returning method named `ConvertToCelsius` that returns a type of `double`. The method should accept one `double` type parameter that represents a temperature in Fahrenheit.
3.  The method body of `ConvertToCelsius` should convert the given temperature in Fahrenheit to Celsius using the following mathematical equation:
    1.  $C = (F - 32) * 5/9$
    2.  Your method should `return` the result of the equation above.
4.  Create a new `static` method named `GetNumber` that returns a type of `double`. The method accepts no parameters. The method should do the following:
    1.  Read a `Line` of user input from the keyboard
    2.  Convert that input into a `double`
    3.  `Return` the value of the user input as a double.
5.  Inside of the `Main()` method, do the following:
    1.  Prompt the user for a temperature in Fahrenheit.
    2.  Use your `GetNumber` method to get the user input as a double.
    3.  Use your `ConvertToCelsius` method to determine the same temperature represented in Celsius.
    4.  Display the temperature in Celsius to the screen.
6.  Ensure that you were able to create and call the methods before advancing.

---

### Part 3: Recursion
1.  Continue the program from before.
2.  Create a `static` method named `Sum` that returns a type of `integer`. The method accepts one parameter of type `Integer`, that should be named `n`.
3.  This method will find the sum of the first `n` positive integers.
    1.  For example, if the parameter `n=5`, then this method would compute: `1+2+3+4+5`
4.  Let’s use our knowledge of the **Commutative Property of Addition** to flip this computation around to the sum of the first `n` positive integers starting with n and counting down to 1.
    1.  For example, if the parameter `n=5`, then this method would compute: `5+4+3+2+1`
5.  Inside of the method body, complete the following:
    1.  If the parameter `n` is equal to 1, then the method should `return a 1`.
    2.  Else the method should `return the Sum(n-1) + n`.
6.  Inside of the `Main()` method of your program, do the following:
    1.  Prompt the user to enter an `integer` value to sum up to.
    2.  Store the user input as the appropriate data type.
    3.  Use your `Sum` method to find the sum of the first `n` numbers as indicated by the user input.
    4.  Display the final sum to the screen.
7.  Ensure that you were able to create and call the method before advancing.

---

### Bonus Challenge: Make A Menu
**(10 pts extra credit on this assignment)**

**THIS FEATURE IS NOT REQUIRED.**

This program is getting pretty long at this point. How could we create a menu to ask the user which of the 3 programs that they would like to execute? If you are feeling confident on how to solve this program, then give it a go!

---

### Submission
Zip up all of your code. Be sure to include the following:
* All `.cs` files
* All `.csproj` files
* Any `.sln` files if your editor generated one or more for you.

Submit your zipped file to the dropbox.

If your submission is rejected by D2L, you can delete the folders "obj" and "bin". They are unnecessary. These folders are where the executable versions of your program are stored.

*Adapted from Professor Jacob Gillenwater, ETSU Dept. of Computing*
