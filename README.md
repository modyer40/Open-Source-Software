# ST211: Open Source Software

<p align="justify">
The practical objective of this course you will learn how to participate in OSS projects
by improving aspects of the software that they feel that they're wrong, suggesting
possible improvement, or just raising issues for the existing solutions.
As a side object of this course you will learn C# which an open source language created by
Microsoft in 2000 and originally started as closed source project and then converted to
an open source project in 2015 as a part of Microsoft's software revolution.
</p>

## Section 0: Recap

### Section Objectives

Part 1 -

- Recap on HTML boilerplate and basics
- Recap on JS syntax and basic programming skills
- Recap on String manipulation

Part 2 -

- Recap on Arrays
- Recap on some Algorithms
- Recap on some Data Structures
- Recap on OOP

### HTML boilerplate

A simple HTML document should start by something like that: -

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <title>Page Title</title>
</head>

<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

<script src="script.js"></script>

</body>

</html>
```

- The `<!DOCTYPE html>` declaration defines that this document is an HTML5 document
- The `<html>` element is the root element of an HTML page
- The `<head>` element contains metadata about the HTML page, such as title, name, description, ...
- The `<title>` element specifies a title for the HTML page (which is shown in the browser's title bar or in the page's
  tab)
- The `<body>` element defines the document's body, and is a container for all the visible contents, such as headings,
  paragraphs, images, hyperlinks, tables, lists, etc.
- The `<h1>` element defines a large heading
- The `<p>` element defines a paragraph
- The `<script>` element specifies some JavaScript code that must be implemented once the element is rendered

### HTML basics

- HTML elements:

```html 
<tagname></tagname>
<tagname>[content]</tagname>
<tagname attribute="value">[content]</tagname>
<tagname attribute1="value" attribute2="value2">[content]</tagname>
```

- HTML self-closing elements:

```html 
<tagname />
```

- [HTML Tags](./htmlcheatsheet.pdf)

### JavaScript basics

- Variables: an abstract storage location paired with an associated symbolic name which contains some known or unknown
  value

```js
var x;
var x = 0;
var x = 'abc';
var x = true;
```

- Arithmetic Operators

| Operator         | Description                                               |
|------------------|-----------------------------------------------------------|
| + (Addition)     | Adds two operands (e.g. x + y)                            |
| - (Subtraction)  | Subtracts the second operand from the first (e.g. x - y)  |
| / (Division)     | Divides the numerator by the denominator (e.g. x / y)     |
| % (Modulus)      | Returns the remainder of an integer division (e.g. x % y) |
| ++ (Increment)   | Increases an integer value by one (e.g. x++)              |
| -- (Subtraction) | Decreases an integer value by one (e.g. x--)              |

- Comparison Operators

| Operator                       | Description                                                                                              |
|--------------------------------|----------------------------------------------------------------------------------------------------------|
| == (Equal)                     | Checks if the value of two operands are equal or not, if equals, returns true (e.g. x == y)              |
| != (Not Equal)                 | Checks if the value of two operands are equal or not, if equals, returns false (e.g. x != y)             |
| \> (Greater than)              | Checks if the value of the left operand is greater than the value in the right (e.g. x > y)              |
| \< (Less than)                 | Checks if the value of the left operand is less than the value in the right (e.g. x < y)                 |
| \>= (Greater than or Equal to) | Checks if the value of the left operand is greater than or equal to the value in the right (e.g. x >= y) |
| \<= (Less than or Equal to)    | Checks if the value of the left operand is less than or equal to the value in the right (e.g. x >= y)    |

- Logical Operators

| Operator           | Description                                              |
|--------------------|----------------------------------------------------------|
| && (Logical AND)   | Returns true if both the operands are true (e.g. x && y) |
| \|\| (Subtraction) | Subtracts the second operand from the first (e.g. x - y) |
| ! (Logical NOT)    | Returns the reverse value of the operand (e.g. !x)       |

- Assignment Operators

| Operator                    | Description                                                                                                                                                                |
|-----------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| = (Simple Assignment)       | Assigns values from the right side operand to the left side operand (e.g. x = 3 + 5)                                                                                       |
| += (Add and Assigment)      | Assigns values from the current value of the left side operand *
plus* the right side operand to the left side operand (e.g. x += 5, equivalent to x = x + 5)               |
| -= (Subtract and Assigment) | Assigns values from the current value of the left side operand *
minus* the right side operand to the left side operand (e.g. x -= 5, equivalent to x = x - 5)              |
| *= (Multiply and Assigment) | Assigns values from the current value of the left side operand *
multiple* the right side operand to the left side operand (e.g. x *= 5, equivalent to x = x * 5)           |
| /= (Divide and Assigment)   | Assigns values from the current value of the left side operand *divided
by* the right side operand to the left side operand (e.g. x /= 5, equivalent to x = x / 5)         |
| %= (Modulus and Assigment)  | Assigns the *reminder* from the current value of the left side operand *divided
by* the right side operand to the left side operand (e.g. x %= 5, equivalent to x = x % 5) |

### Functions

A function is a group of statements which can be called to accomplish a specific task. The function usually has the
following criterias: -
* NAME: a special name that we give to the function to call it with.
* Return Value (Optional): a value that the function will give back after it finishes executions.
* Parameters (Optional): a number of values that the function takes to be able to accomplish a specific task.

```js
// Function called log with no parameters and no return value
function log() {
    console.log('Hello, World!');
}

// Function called log with one parameter and no return value
function log(name) {
    console.log('Hello, ' + name);
}

// Function called sum that takes two parameters and a return value
function sum(x, y) {
    return x + y; // Return statement that returns a value
}
```

- Prebuilt Functions: functions that already exists in JavaScript that we can use to do specific tasks.

| Function | Description                                    | Parameters                                            |
|----------|------------------------------------------------|-------------------------------------------------------|
| `prompt` | a function that asks the user to enter a value | `message`: a message to show to the user as a hint    |
| `alert`  | a function that sends a message to the user    | `message`: a message to show to the user as an output |

### Control Flow

Control Flow is the order in which the computer executes statements in a script; using a condition which is usually an
boolean expression.

- Conditional Statements: the first type of control flow statements which specify if a specific block of code will be
  executed or not.

```js
// If Statement
if (condition) {
    // running code in case condition is true
}

// If-Else Statement
if (condition) {
    // running code in case condition is true
} else {
    // running code in case condition is false
}

// If-ElseIf-Else Statement
if (condition1) {
    // running code in case condition1 is true
} else if (condition2) {
    // running code in case condition1 is false && condition2 is true
} else {
    // running code in case condition1 is false && condition2 is false
}
```

```js
// Switch Statement
switch (expression) {
    case value1:
        // running code in case expression == value1
        break;

    case value1:
        // running code in case expression == value2
        break;

    default:
    // running code in case non of the values matches the expression
}
```

- Loops: the second type of control flow statements which specify how many times a specific block of code will be
  executed.

```js
// For Loop
for (pre_statement; condition; post_statement) {
    // running code in case condition is true
}

// pre_statement: a regular js statement that will be called before the loop starts
// post_statement: a regular js statement that will be called after each iteration
```

```js
// While Loop
while (condition) {
    // running code in case condition is true
}
```

```js
// Do-While Loop
do {
    // normal running code
} while (condition); // re-execute the previous block if the condition is true
```

### Strings

Strings are a group of characters stored together denoted by single or double quotes (e.g. `var x = 'abc';`
or `var x = "abc";`)

- Properties: -

| Property | Description                      | Syntax                    |
|----------|----------------------------------|---------------------------|
| `length` | returns the length of the string | `'abc'.length`: returns 3 |

- Member Functions (Methods): -

| Method        | Description                                                                                                                                                                                                                | Syntax                                 |
|---------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------|
| `charAt`      | returns the character at the specified index                                                                                                                                                                               | `'abc'.charAt(1)` returns 'b'          |
| `charCodeAt`  | returns a number indicating the ASCII code of the character at the specified index. Refer to [ASCII Table](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1b/ASCII-Table-wide.svg/1200px-ASCII-Table-wide.svg.png) | `'abc'.charCodeAt(1)` returns 98       |
| `concat`      | returns a string resulting from combining two strings                                                                                                                                                                      | `'abc'.concat('def')` returns 'abcdef' |
| `indexOf`     | returns the index of the first occurence of the specified value, or -1 if it doesn't exist                                                                                                                                 | `'abc'.indexOf('b')` returns 1         |
| `lastIndexOf` | returns the index of the last occurence of the specified value, or -1 if it doesn't exist                                                                                                                                  | `'abbc'.lastIndexOf('b')` returns 2    |
| `slice`       | returns an extracted section of the string                                                                                                                                                                                 | `'abbc'.slice(0, 2)` returns 'ab'      |
| `toLowerCase` | returns the lower case version of the string                                                                                                                                                                               | `'ABC'.toLowerCase()` returns 'abc'    |
| `toUpperCase` | returns the upper case version of the string                                                                                                                                                                               | `'abc'.toUpperCase()` returns 'ABC'    |

- Static functions: -

| Function       | Description                                          | Syntax                                |
|----------------|------------------------------------------------------|---------------------------------------|
| `fromCharCode` | returns the character from the specified ASCII value | `String.fromCharCode(97)` returns 'a' |

- Custom Operators: -

| Operator | Description                   | Syntax               |
|----------|-------------------------------|----------------------|
| +        | Converts the string to number | `+'100'` returns 100 |


### Arrays

The array is a data structure that lets you store multiple values in a single variable accessed by indices.

- Syntax: -

```js
// Initialization
var names = new Array("ibrahim", "gamal", "mohamed");
// Or, a better way
var names = ["ibrahim", "gamal", "mohamed"];

// Accessing variables
names[0] = "ibrahim"
names[1] = "gamal"
names[2] = "mohamed"
```

- Properties: -

| Property | Description                     | Syntax                        |
|----------|---------------------------------|-------------------------------|
| `length` | returns the length of the array | `[1, 2, 3].length`: returns 3 |

- Member Functions (Methods): -

| Method        | Description                                                                                          | Syntax                                         |
|---------------|------------------------------------------------------------------------------------------------------|------------------------------------------------|
| `push`        | adds one or more elements to the end of the array and returns the new length of the array            | `[1, 2].push(3)` returns 3, arr = [1, 2, 3]    |
| `unshift`     | adds one or more elements to the start of the array and returns the new length of the array          | `[1, 2].unshift(3)` returns 3, arr = [3, 1, 2] |
| `pop`         | removes the last element from the array and returns it                                               | `[1, 2].pop()` returns 2                       |
| `shift`       | removes the first element from the array and returns it                                              | `[1, 2].shift()` returns 1                     |
| `includes`    | returns a boolean indicating whether the value exists or not                                         | `[1, 2, 3].includes(2)` returns true           |
| `indexOf`     | returns the index of the first occurence of the specified value, or -1 if it doesn't exist           | `[1, 2, 3].indexOf(2)` returns 1               |
| `lastIndexOf` | returns the index of the last occurence of the specified value, or -1 if it doesn't exist            | `[1, 2, 2, 3].lastIndexOf(2)` returns 2        |
| `join`        | returns a string resulted from joining all the elements in the array separated by a specific element | `[1, 2, 3].join('')` returns '123'             |
| `reverse`     | returns a reversed version of the array                                                              | `[1, 2, 3].reverse()` returns [3, 2, 1]        |
| `slice`       | returns a subarray from the original array                                                           | `[1, 2, 3].slice(1, 3)` returns [2, 3]         |
| `splice`      | returns a subarray from the original array and removes it from the original                          | `[1, 2, 3].splice(1, 1)` returns [2]           |
| `sort`        | returns a sorted array                                                                               | `[3, 2, 1].sort()` returns [1, 2, 3]           |

### Objects

Objects are composed of attributes. If an attribute contains a function, it is considered to be a method of the object,
otherwise the attribute is considered a property.

- Syntax: -

```js
var person = new Object({
  fullName: 'Ibrahim Gamal',
  eat: function () {
      console.log('Eating ...');
  }
});
// Or
var person = {
  fullName: 'Ibrahim Gamal',
  eat: function () {
      // 'this' is keyword used to access an object within a context
      console.log(this.fullName + ' is eating ...');
  }
}

// Accessing attributes
person.fullName = 'Ibrahim Gamal'
person.eat()
// Or
person['fullName'], person['eat']()
```

### Classes

Classes are templates for Objects.

- Syntax: -

```js
// Creation
class Person {
    constructor(fullName) {
        this.fullName = fullName;
    }
    
    eat() {
      // 'this' is keyword used to access an object within a context
      console.log(this.fullName + ' is eating ...');
    }
}

// Usage
var ibrahim = new Person('Ibrahim Gamal');

// Accessing attributes
ibrahim.eat()
```

### Algorithms

An algorithm is a procedure used for solving a problem or performing a computation. Algorithms act as an exact list of
instructions that conduct specified actions step by step in either hardware- or software-based routines.

### Common Algorithms' Pseudocode

- Binary Search: a fast search algorithm with time complexity of Ο(log n) that works only with sorted arrays

```
A = sorted array
n = size of array
x = value to be searched

low = 1
high = n 

while low >= high
   mid = low + ( high - low ) / 2
   
   if A[mid] < x
      low = mid + 1
      
   if A[mid] > x
      high = mid - 1 

   if A[mid] = x 
      return mid
```

- Insertion Sort: an efficient algorithm for sorting a small number of elements.

```
A = array
for i = 2 to length[A]
     key = A[i]
     j = i - 1
     while j > 0 and A[j] > key
        A[j + 1] = A[j]
        j = j - 1
     A[j + 1] = key
```

### Task 1: HTML boilerplate

```
Create a web page that meets the following criterias: -
1) Has your NAME as the title
2) Has the COURSE_NAME in a large heading
3) Has your NAME in a paragraph
4) Renders a 'script.js' file 
```

### Task 2: Greeting with the user's name

```
Create a web page that do the following: -
1) Asks the user for this name in a dialog
2) Outputs a welcome message with this name in another dialog

Example:
IN> Ibrahim
OUT> Welcome, Ibrahim!
```

### Task 3: Square of a number

```
Create a web page that do the following: -
1) Asks the user for a number in a dialog
2) Outputs the square of that number in another dialog

Example:
IN> 2
OUT> 4
```

### Task 4: Average of two integers

```
Create a web page that do the following: -
1) Asks the user for two numbers in a dialog
2) Outputs the average of these two numbers in another dialog

Example:
IN> 2
IN> 4
OUT> 3
```

### Task 5: Adding N integers

```
Create a web page that do the following: -
1) Asks the user for a number (N) in a dialog
2) Asks the user for others numbers N times in a dialog
3) Outputs the N numbers in another dialog

Example:
IN> 3
IN> 1
IN> 2
IN> 3
OUT> 6
```

### Task 6: Converting Celsius to Fahrenheit

```
Create a web page that do the following: -
1) Asks the user for a number (C) in a dialog
2) Outputs the corresponding value of this number in fahrenheit in another dialog

Example:
IN> 40
OUT> 104
```

### Task 7: Converting String to Uppercase (2 methods)

```
Create a web page that do the following: -
1) Asks the user for a string in a dialog
2) Outputs the upper case of this string in another dialog

Example:
IN> ibrahim
OUT> IBRAHIM
```

### Task 8: Adding string ranks

```
Create a web page that do the following: -
1) Asks the user for a string in a dialog
2) Outputs the sum of the string characters' ranks in the alphabtical order in another dialog

Example:
IN> abc
OUT> 6

Explanation:
a = 1, b = 2, c = 3
```

### Task 9: Max Number

```
Create a web page that do the following: -
1) Asks the user for the length of an array in a dialog
2) Asks the user for each value in the array in a dialog
2) Outputs the max of the array in another dialog

Example:
IN> 3
IN> 1
IN> 2
IN> 3
OUT> 3
```

### Task 10: Last Even Number

```
Create a web page that do the following: -
1) Asks the user for the length of an array in a dialog
2) Asks the user for each value in the array in a dialog
2) Outputs the last even number in the array in another dialog

Example:
IN> 3
IN> 1
IN> 2
IN> 3
OUT> 2
```

### Task 11: Implement Binary Search

### Task 12: Implement Insertion Sort

### Task 13: Reverse a LinkedList

```
Create a web page that do the following: -
1) Asks the user for the length of an array in a dialog
2) Asks the user for each value in the array in a dialog
2) Outputs the array in a reversed order in another dialog

Example:
IN> 3
IN> 1
IN> 2
IN> 3
OUT> 3 2 1
```

### Task 14: Most Frequent Number

```
Create a web page that do the following: -
1) Asks the user for the length of an array in a dialog
2) Asks the user for each value in the array in a dialog
2) Outputs the most frequent number and the number of frequency in another dialog

Example:
IN> 5
IN> 1
IN> 2
IN> 3
IN> 4
IN> 2
OUT> 2 with frequency of 2
```
