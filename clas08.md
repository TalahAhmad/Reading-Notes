# 08- Operators and Loops

## Expressions and Operators

- expression is valid unit of code that resolves value

- two types of expressions: those that have side effects (such as assigning values) and those that purely evaluate
    x = 7 is an example of the first type
    = is the op
    x is variable
    expression evalautes to 7

- second type: 
    3 + 4
    + operator to add 3 and 4 together and produces a value, 7. 
        However, if it's not eventually part of a bigger construct 

### Comparison Ops

- compares its operands and returns a logical value based on whether the comparison is true

- can be numerical, string, logical, or object values

-**string**: compared based on standard lexicographical ordering, using Unicode values

- if operands arent same type, js will try to convert them appro. // they're usually numbers

- exceptions: involve the === and !== operators, which perform strict equality and inequality comparisons
    they do attempt to convert the operands before checking equality

### Assignment Ops

- assigns a value to its left operand based on the value of its right operand

- simple assignment op: = (assigns something to the right which goes to the left operand)

- x = f() is an assignment expression that assigns the value of f() to x

#### Assigning to Properties

- expression evaluates to an object, then the left-hand side of an assignment expression may make assignments to properties of that expression
    let obj = {};

    obj.x = 3;
    console.log(obj.x); // Prints 3.
    console.log(obj); // Prints { x: 3 }

    const key = "y";
    obj[key] = 5;
    console.log(obj[key]); // Prints 5.
    console.log(obj); // Prints { x: 3, y: 5 }

- If an expression does not evaluate to an object, then assignments to properties of that expression do not assign
    let val = 0;

    console.log(val.x = 3); // Prints 3.
    console.log(val.x); // Prints undefined.
    console.log(val); // Prints 0.

#### Destructuring

- expression that makes it possible to extract data from arrays or objects using a syntax that mirrors the construction of array and object literals (combines arrays)
    const foo = ['one', 'two', 'three'];

// without destructuring
const one   = foo[0];
const two   = foo[1];
const three = foo[2];

// with destructuring
const [one, two, three] = foo;

#### Evaluating and nesting

- used within a variable declaration (i.e., with const, let, or var) or as standalone statements)
// Declares a variable x and initializes it to the result of f().
// The result of the x = f() assignment expression is discarded.
let x = f();

x = g(); // Reassigns the variable x to the result of g().

- become a result value although scarcely used

- its result can itself be assigned to another variable. It can be logged, it can be put inside an array literal or function call, and so on

#### Avoid Assignment Chains

- putting a variable chain in a const, let, or var statement often does not work
    let z = y = x = f();

## Loops and Iterations

### For statement

- A while loop 

set a condition this code
enter the loop and check
if it does execute then true
then check the code
if it doesn't, the loop will break it'll run the next

A for loop

initial value
if it evals to true, execute code then increment then start all over
if it doesnt executed the loop, go to next code

while loop
let x = 0;
 while (x < 10){
   console.log(x);
   x++
increment x by 1
these numbers are less than 10 it stopped at 9
