# Lesson 1 - Introduction, Setup and Version Control

### Projected Time

About 2 hours

### Prerequisites

- Basic knowledge of HTML and CSS
- IDE (preferably Visual Studio Code editor)
- Netlify account
### Motivation

JavaScript is used on the frontend of almost every website. It's also a widely-used scripting language that be used on the backend as well. The JavaScript lessons set a solid foundation in JavaScript basics so we can use the language in more robust ways in later lessons.

### Lesson

JavaScript is a scripting language used to make webpages interactive.

`HTML` controls the structure of the webpage.
`CSS` controls the way the webpage is presented.
`JS` helps make your web page interactive. For example, respond to button clicks, etc.
Combining all three together is when your webpage comes to life.

Note: Java and JavaScript are not the same. Java is a programming language whereas JavaScript is a scripting language.

#### JavaScript Concepts

- JS expressions
    -  is a valid set of literals and expressions that evaluate to a single value that is an expression.
    For example: 5 + 5 = 10
- JS statements
    - is used to control the flow of a script or a programhe and rely on conditions.
    For example: `if(something) {display something} else {display somethingelse}`
- JS identifiers
    - are names that are given to entities like variables, functions, class, etc.
    For example: `const a = 'hello';` OR `const _a = 'hello';`
    - They cannot start with a number but can start with _ and preferably camelCase.
- JS keywords
    - are reserved words that cannot be used as an identifier.
    For example: `this`, `break`, `let`, `if`, `else`
- JS operators
    - perform some operations like arithmetic (+), assignment (=), comparison (==, <, >), etc.

#### Comments
Comments can be used to explain JavaScript code, and to make it more readable. They can either be:
 - single-line: `// Some comment here`
 - multi-line:
    ```
    /*
    The code below will change
    the heading with id = "myH"
    and the paragraph with id = "myP"
    in my web page:
    */
    ```
#### JavaScript Conventions
Coding conventions are style guidelines for programming.
- Case Sensitive - JavaScript is a case-sensitive language.
- Naming conventions - all variables, identifiers and function names can either be camelCase or PascalCase.
- No use of hyphens - They are considered a subtraction expression.
- Brackets - All brackets have a specific way of being used in javascript.
    - () : used for functions or to surround conditional statements. Most popular of the brackets.
    Example: `(5 + 5)`
    - {} : wrap blocks of code. 
    Example: `if (expertCoder) {console.log(“Yes”)} else {console.log(“No”)}`
    - [] : used in arrays or objects.
    Example: `[“apple”, “banana”, “kiwi”]`
    - <> : HTML elements like `<h1>`, `<html>`, etc
- Semicolon: Every statement in JS ends with a semicolon. Optional but highly recommended.
    Example: `console.log("Hello");`

#### console.log
`console.log` is highly used for debugging in JavaScript. It has no impact on the page but shows up in our console in developer tools.

```console.log("Hello")```
Prints the string "Hello" in the console.

```console.log(Hello)```
Throws an error because it isn't enclosed in `""`.

```console.log(45)```
Prints the number 45 in the console.

```console.log("45")```
Prints the string "45" in the console.

```console.log("Hello" + "world")```
Prints the string "Helloworld" in the console.

```console.log(45 + 1)```
Prints the number 46 in the console.

```alert("Hello")```
Prints the string "Hello" in the dialog box in your browser.

You can use the console in the developer tools of your browser to play around with some JavaScript code.

#### Visual Studio Code extenstions
Some very useful extensions in Visual Studio Code for JavaScript are:
- [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint): Linting is the automated checking of your source code for programmatic and stylistic errors.
- [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode): JavaScript formatter. It removes all original styling and ensures that all outputted JavaScript conforms to a consistent style.
- [Night Owl](https://marketplace.visualstudio.com/items?itemName=sdras.night-owl): to make your code look beautiful with colors.

#### Git
Git is mainly used for version control. Version control is the practice of tracking and managing changes to software code.
Some [Git commands](/git/git-commands.md) to get you started.

### Supplemental Materials

- [The JS Way](https://github.com/thejsway/thejsway)
- [Hello World](https://javascript.info/hello-world)
