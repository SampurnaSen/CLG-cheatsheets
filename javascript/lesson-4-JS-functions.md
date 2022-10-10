# Lesson 4 - JavaScript Functions

### Projected Time

About 2 hours

### Lesson

#### Functions

Functions are one of the fundamental building blocks in JavaScript. It's a set of statements that performs a task or calculates a value. We begin by writing the “function” keyword and then giving it a name. Then we add parentheses (this is where our parameters go in), followed by curly braces. This is the body of the function. We then call the function/invoke the function.

- Function declaration: Declared functions are not executed immediately. They are "saved for later use", and will be executed later, when they are invoked (called upon).
```
function greet() {
  // body of the function
  console.log(“Hey there!”);
}
greet();
```
- Function expression: A function expression can be stored in a variable. Functions stored in variables do not need function names. They are always invoked (called) using the variable name.
```
let greetings = function() {
  console.log(“Hey there!”);
}
greetings();
```

Function declarations in JS are `hoisted`, meaning it’s moved to the first order of business before the rest of the JS code execution.
```
greetings(); // invoking before declaration

function greetings() {
  console.log(`Helly there!`);
}
```

#### Naming convention
- Function names are always in lowerCamelCase
- They should preferably start with a verb (For example, `getName()`, `findSum()`)

#### Arguments and Parameters
Both arguments and parameters are used interchangeably in JavaScript functions but the main difference is that `parameters` identify values that are passed into a function. For example, a function to add three numbers might have three parameters. A function has a name, and it can be called from other points of a program. When that happens, the information passed is called an `argument`.
```
// "name" is the parameter
function catName(name) {
  console.log(`My cat's name is ${name}`);
}
// "Tiger" is the argument
catName("Tiger");
```

#### Return statement
Return statement is a statement used to return a value. One thing to keep in mind is that a function stops executing once it reaches the “return” statement. So always place “return” at the end. When a function returns a value, it then jumps to the previous place in the flow of control.
```
function compare(a, b) {
    if (a > b) {
        return -1;
    } else if (a < b) {
        return 1;
    }
    return 0;
}
compare(6, 9)
console.log(‘Executed after comparison`);
```
If a function does not have a return statement then it returns undefined. Always have a return statement or a console.log/alert in a function.

### Supplemental Materials

- [Function basics](https://javascript.info/function-basics )
- [w3schools JS function](https://www.w3schools.com/js/js_function_definition.asp)
- [JavaScript for new programmers](http://jsforcats.com/)
- [Demo using functions](https://github.com/SampurnaSen/findLargerNumber)