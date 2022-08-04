# 07 - Programming with JavaScript

## Control Flow

- order  in which the computer executes statements in a script

- code is run from first line to last line unless
    quite frequently conditionals and loops are involved

- conditional structure: if...else // different code executes dependant on whether the for is complete or not
    if (field==empty) {
    promptUser();
} else {
    submitForm();
}

- typical JS  script includes many control structures, including conditionals, loops, and functions

- dictate complex flows of processing even with only a few lines of code
    means when you read a script // read from beginning to end, look at program structure and how it affects order of execution

## JS Functions

- function is a block of code designed to perform a particular task
    executed when something evokes it (calls it)
    ex: unction myFunction(p1, p2) {
  return p1 * p2;   // The function returns the product of p1 and p2
}

### JS Function Syntax

- function is defined with // **function**, a name, followed by **()**
    can contain letters, underscores, and dollar signs
    parantheses may include parameters seperated by commas: (p1,p2,p3...)
    the code to be executed is put in side curly brackets **{}**
    ex: function name(parameter1, parameter2, parameter3) {
  // code to be executed
}

- parameters are listed inside the parantheses in the function definition (behave as local variables)

- arguments are the values by the function when it is invoked

### Function Invocation

- code inside will executed when it is **invoked** 
    When an event occurs (when a user clicks a button)
    When it is invoked (called) from JavaScript code
    Automatically (self invoked)

### Function Return

- return statement // function will sop executing

- if function was invoked from a statement JS will return to execute the code after

-return value // _returned_ back to the _caller_

### WHhy Functons?

- define the code, use it many times // use the same code many times with diferent argumnts to produce diff results

function toCelsius(fahrenheit) {
  return (5/9) * (fahrenheit-32);
}
document.getElementById("demo").innerHTML = toCelsius(77);
    toCelsius refers to the function object, and toCelsius() refers to the function result

### The () Operator Invokes the Function

- Accessing a function without () will return the function object instead of the function result.

### Functions used as Variable Values

- used the same way as you use variables, in all types of formulas, assignments, and calculations

- Instead of using a variable to store the return value of a function:

let x = toCelsius(77);
let text = "The temperature is " + x + " Celsius";
You can use the function directly, as a variable value:

let text = "The temperature is " + toCelsius(77) + " Celsius";

### Local Variables

- variables declared w/in the JS function become **LOCAL** to the function
    can only be accessed w/in the function
    variables with the same name can be used in different functions
    created when a function starts and deleted when the function is completed

## JS Ops

- assign values to varibales and add them together // 
    let x = 5;         // assign the value 5 to x
    let y = 2;         // assign the value 2 to y
    let z = x + y;     // assign the value 7 to z (5 + 2)

- **Assignment op** (=) assigns a value to a variable // let x = 10;

Operator	Description
+	Addition
-	Subtraction
*	Multiplication
**	Exponentiation (ES2016)
/	Division
%	Modulus (Division Remainder)
++	Increment
--	Decrement

Operator	Example	Same As
=	x = y	x = y
+=	x += y	x = x + y
-=	x -= y	x = x - y
*=	x *= y	x = x * y
/=	x /= y	x = x / y
%=	x %= y	x = x % y
**=	x **= y	x = x ** y

### JS String Ops

- + can also be used to concatenate strings
    let text1 = "John";
let text2 = "Doe";
let text3 = text1 + " " + text2;
The result of text3 will be: John Doe

- The += assignment operator can also be used to add (concatenate) strings:
    let text1 = "What a very ";
text1 += "nice day";
The result of text1 will be: What a very nice day

- When used on strings, the + operator is called the concatenation operator

JS Comparison Ops
Operator	Description
==	equal to
===	equal value and equal type
!=	not equal
!==	not equal value or not equal type
>	greater than
<	less than
>=	greater than or equal to
<=	less than or equal to
?	ternary operator

### JS Adding Strings and Numbers

- Adding two numbers, will return the sum, but adding a number and a string will return a string
    let x = 5 + 5;
let y = "5" + 5;
let z = "Hello" + 5;
The result of x, y, and z will be:
10
55
Hello5