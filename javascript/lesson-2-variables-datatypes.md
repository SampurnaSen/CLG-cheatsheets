# Lesson 2 - Variables and Data Types

### Projected Time

About 2 hours

### Prerequisites

- GitHub account
- VS Code setup

### Lesson
#### Variables
Variables are like containers, they store data and can be later used in our code.
- let: variables can be reassigned. ```let car = “Subaru Outback”;```
- const: variable cannot be reassigned, it’s a constant.```const carOwner = “John Doe”;```

You can declare first and initialize later for let but not for const.
```
let car;
car = “Subaru Outback”;
```

`Declare a variable`: we flag the name for later use
`Initialise a variable`: assign a value to the variable

#### Block scope
Block scope restricts the variable that is declared inside a specific block, from access by the outside of the block. (Any statement within curly braces {}).
- Global scope: anything declared outside the scope block or function.
- Local scope: declared within the block or function.

```
/* program to show the change in global variable */
let greetMessage = "hello";

function greet() {
    greetMessage = 3; //re-initialising in a local scope
}

// before the function call
console.log(greetMessage);

//after the function call
greet();
console.log(greetMessage); // 3
```

```
/* program showing local scope of a variable */
let greetMessage = "hello";

function greet() {
    let worldMessage = "World"; //declaring & initialising a variable in local scope
    console.log(greetMessage + worldMessage);
}

greet();
console.log(greetMessage + worldMessage); // error
```

Some common console methods are:
- `console.log(“Hey ” + “there!”);` - to log something in the console.
- `console.error(“Name field is required!”);` - errors are shown in red.
- `console.warn(“This is a warning”);` - warnings are less severe and shown in yellow.
- `console.clear();` - clears the web console.

#### Data Types
Data type is a classification that specifies which type of data/value is stored in our variable. JavaScript is `loosely typed` - you don't have to specify the data type in advance.

`Primitive data` types are pre-defined:
- String
    - Template literals are enclosed by backtick
    ```
    let myString = `Hey there!`;
    let myString = `Hey there!
                    My name is Jane Doe`;
    let myString = `Jane said, “Hello ladies!”`;
    let myString = `My name is ${name}`; //string interpolation
    ```
- Number
- Boolean `let isNum = false;`
- Null: It is the intentional absence of the value
```
let name;
console.log(name); // undefined
```
- Undefined - It means the value does not exist
```
let number = null; //null
```

`Non-primitive` data type is not pre-defined:
- Object: an entity with properties and methods(functions).
```
const name = “Jane”;
console.log(name.length); // property of object "name"
console.log(name.toUpperCase()); // method of object "name"
```

More examples:
```
let carModel = "Jaguar XF";
let carOwner = "Jane";
let ownerStatement = "The owner of this ${carModel} car is ${carOwner}"
console.log(ownerStatement);
let statementUpper = ownerStatement.toLocaleUpperCase();
let statementlength = statementUpper.length;
console.log(statementlength);
```

### Supplemental Materials

- [MDN Webdocs](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
- [JS Variables](https://javascript.info/variables)
