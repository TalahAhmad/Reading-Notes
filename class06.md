# 06 - Dynamic web pages with JavaScript

## JavaScript

- just-in-time lang. with first class functions

- known as scripting language for web pages

- also used by non-browser environments such as Node.js, adobe acrobat, etc.

- standards are  ECMAScript Language Specification (ECMA-262) and the ECMAScript Internationalization API specification (ECMA-402)

## Input and Output of JavaScripts

## JS Variables

- 4 ways to declare a variable:

    var
    let
    const
    nothing

### What are variables

- containers for storing data
    ex: x, y, and z, are variables, declared with the var keyword
    var x = 5;
    var y = 6;
    var z = x + y;
    ex: In this example, x, y, and z, are variables, declared with the let keyword
    let x = 5;
    let y = 6;
    let z = x + y;
    ex: In this example, x, y, and z, are undeclared variables
    x = 5;
    y = 6;
    z = x + y;

#### When to use var 

- always declare variables with var, let and const

- var is used in JS code from '95-'15

- let and const were in '15

- **if you're using an older browser** use var

#### When to use JS const

- general rule: **always declare variables w const**

- **if the value can change**, use let
    const price1 = 5;
    const price2 = 6;
    let total = price1 + price2
    two variables declared w const (constant cannot be changed)
    total is declared w let (value can be changed)

#### JS identifiers

- **all variables must be identified w unique names**

-unique names are called **identifiers**
    can be shprt names (x,y) or descriptive names (age, sum, totalVolume)

    - rules for structuring a name for unique identifiers (variables):
    Names can contain letters, digits, underscores, and dollar signs.
    Names must begin with a letter
    Names can also begin with $ and _ (but we will not use it in this tutorial)
    Names are case sensitive (y and Y are different variables)
    Reserved words (like JavaScript keywords) cannot be used as names

#### The Assignment Op

- = is an **assignment** op not an "equal to" op
    x = x + 5
    makes sense in JS: it assigns the value of x + 5 to x

- in JS the op is written like ==

#### JS Date Types

- can hold numbers like 100 and text values like "John Doe"

- strings: text values
    
- Strings are written inside double or single quotes. Numbers are written without quotes.

- If you put a number in quotes, it will be treated as a text string
    const pi = 3.14;
    let person = "John Doe";
    let answer = 'Yes I am!';

#### Declaring a JS Variable

- declare a variable w var and let
    var carName;
        or
    let carName;
    after the declaration the variable has no value
    to assign a value, use the equal sign:
    carName = "Volvo";

- You can also assign a value to the variable when you declare it:
    let carName = "Volvo";

- **good programming practice to declare all variables at the beginning of a script**

#### One Statement, Many Variables

- you can declare many variables in one statement

- start the statement with let and separate the variables by comma 
    let person = "John Doe", carName = "Volvo", price = 200;

- a declaration can span multiple lines
    let person = "John Doe",
    carName = "Volvo",
    price = 200;

#### Value = undefined

- variables are often declared without a value

- 