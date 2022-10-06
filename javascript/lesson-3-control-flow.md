# Lesson 3 - Control Flow

### Projected Time

About 2 hours

### Lesson

#### Operators
Operators are used in expressions to perform specific actions. An operator is capable of manipulating a certain value or operand.
What is an operand?
Operands combine with operators to write expressions. `[Example: 2 + 5  (2 & 5 are operands; + is the operator)]`

Types of operators:
- Arithmetic operators
    - +	Addition / Concatenation
    - -	Subtraction
    - *	Multiplication
    - /	Division
    - %	Modulus (Division Remainder)
    - ++ Increment
    - -- Decrement
- Assignment operators
    - `=`
    - `+=` 
    - `-=`
- Comparison operators
    - `==`	equal to
    - `!=`	not equal
    - `>`	greater than
    - `<`	less than
    - `>=`	greater than or equal to
    - `<=`	less than or equal to
- Logical operators
    - `&&`    and
    - `||`    or
    - `!`     not
- Conditional operators
    - `variablename = (condition) ? value1: value2`
- Typeof operators
    - `typeof "Hello"`
    - `typeof 45`
    - `typeof true`
- Unary operator: one operand
    - `typeof "John"`
- Binary operator: two operands
    - `2 + 2`
- Ternary operator: three operands
    - `variablename = (condition) ? value1: value2`

#### Truthy Falsy
Truthy evaluates to true. Falsy evaluates to false.
Falsy: false, 0, empty strings, null undefined, and NaN
Truthy: all other values

#### Control Flow
Control flow is the order in which our code is executed. Originally, code executes in a top-down manner, unless the code control changes its course when it meets with other structures such as: 
- Loops: iteration statements; it repeats the given task until the given condition is met
```
// program to display text 5 times
const n = 5;

// looping from i = 1 to 5
for (let i = 1; i <= n; i++) {
    console.log(`I love JavaScript.`);
}
```
- Conditional statements: decision making statements
```
const isMailSent = true;

if (isMailSent) {
  console.log('Mail sent to recipient');
} else {
   console.log('Mail is not sent to recipient');
}
```
- Functions: a block of code that is reusable
```
function greetings() {
  console.log("Hey there!");
}
greetings();
```

### Supplemental Materials

- [Operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)
- [Conditional Statements](https://www.w3schools.com/js/js_if_else.asp)
- [You don't know JS](https://github.com/getify/You-Dont-Know-JS/blob/2nd-ed/scope-closures/README.md)
