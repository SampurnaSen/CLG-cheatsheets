# Lesson 8 - Arrays and Loops

### Projected Time

About 2 hours

### Lesson

#### Arrays
Arrays are used to group similar types of values together. Each value is called an element specified by an index. Arrays are similar to objects but arrays use numbered index, whereas objects use named index.

```
/* Array: indexing starts from 0 */
["oranges", "bananas", "grapes"] // 0=>oranges; 1=>bananas; 2=>grapes

/* Object: indexing is by name */
{
 name: "Jane",
 age: 25
}
```

#### Declaring an arrays
We will create an array using the array literal notation.

`let colors = ['red', 'green', 'blue'];` - holding string elements.
`const numberArray = [ 2, 4, 6, 8];` - holding number elements.
`let fruits = [];` - empty array

#### Retrieving/Accessing an arrays
JavaScript arrays are zero-based indexed.

```
let colors = ['red', 'green', 'blue'];
// colors[0] => return "red"
// colors[1] => return "green"
```

#### Working with arrays
- length - the length property of an array returns the number of elements.
```
let colors = ['red', 'green', 'blue'];
console.log(colors.length);
```
- push() - To add an element to the end of an array, you use the push method.
```
let seas = ['Black Sea', 'Caribbean Sea', 'North Sea', 'Baltic Sea'];
seas.push('Red Sea');
console.log(seas);
```
- pop() - To remove an element from the end of an array, you use the pop method.
```
let seas = ['Black Sea', 'Caribbean Sea', 'North Sea', 'Baltic Sea'];
seas.pop();
console.log(seas);
```
- sort() - sorts the elements alphabetically in strings and in ascending order
```
let numberArray = [5, 2, 7, 4];
numberArray.sort();
```
- find() - returns the first value of an array element that passes a test.
```
const numberArray = [ 2, 4, 6, 8];
function checkNum(numberArray) {
  return numberArray > 5;
}

function myFunction() {
  console.log(numberArray.find(checkNum)); //first number
}
myFunction();
```
- filter() - creates a new array filled with elements that pass a test provided by a function.
```
const numberArray = [ 2, 4, 6, 8];
function checkNum(numberArray) {
  return numberArray > 5;
}

function myFunction() {
  console.log(numberArray.filter(checkNum)); //first number
}
myFunction();
```

#### Loops
Loops repeatedly perform an action until we tell it to stop. They are used to execute a piece of code a desired number of times.

- for loop: 
  - executes a block of code as long as a specified condition is true.
  - It takes three arguments: initialization, condition, and increment.
  ```
  for (let i = 0; i < 5; i++) {
    console.log("The number is " + i + "<br>");
  }
  ```
- forEach loop
  - This method calls a function for each element in an array.
  ```
  const fruits = ["apple", "orange", "banana"];
  fruits.forEach(myFunction);
  function myFunction(item) {
      console.log(item);
  }
  ```
- while loop
  - The while loop loops through a block of code as long as a specified condition is true.
  ```
  let n = 0; //initialisation
  while (n < 3) { //condition
    n++; //iteration or increment
  }
  console.log(n);
  ```


### Supplemental Materials

- [JavaScript Arrays](https://www.w3schools.com/js/js_arrays.asp)
- [Arrays](https://javascript.info/array)
- [Exercise on loops](https://www.w3schools.com/js/exercise_js.asp?filename=exercise_js_loops1)