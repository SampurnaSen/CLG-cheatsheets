# Lesson 7 - JavaScript Objects

### Projected Time

About 2 hours

### Lesson

#### Objects
Object is a standalone entity. It can be viewed as a container that contains some properties and variables. Objects also have a type and the type can be date, string, number, boolean, etc. A JS object has a collection of properties associated with it. A property of an object can be explained as a variable that is attached to the object. You access the properties of an object with a simple dot-notation.

```
userDetails.firstName = "Melina"; //userDetails=>object; firstName=>property; Melina=>value
userDetails.lastName = "Dorsey"; //string
userDetails.age = 25; //number
userDetails.isActive = true; //boolean
userDetails.getDetails() {} //function
```

#### Declare an object
There are different ways in which you can declare an object. We will stick to only one.

```
let userDetails = {}; //using let
const userDetails = {}; //using const
```

Then we fill out our details inside the block using key-value pairs. Key is the property and value is the value set for that property.

```
let userDetails = {
  firstName: "Melina",
  lastName: "Dorsey",
  age: 25,
  isActive: true,
  address: {
    houseNumber: 2,
    street: "Abby street"
  },
  getDetails: function() {
    console.log("Hello");
  }
}
```

#### Retreive an object
Now that we have declared our object, let’s go ahead and retrieve or fetch some of these properties.

```
userDetails.firstName; // using dot notation
userDetails[‘firstName’]; // using square brackets
```

#### "this" keyword
"This" keyword is a reserved JavaScript keyword. It basically refers to an object. It’s commonly used inside object methods to grab the properties of its parent object.

```
let userDetails = {
  firstName: “Melina”,
  lastName: “Dorsey”,
  age: 25,
  getDetails: function() {
    console.log(`Name is ${this.firstName}, age is ${this.age}`);
  }
}
```

#### JSON
JSON expands to JavaScript Object Notation. It’s not the same as JavaScript but looks very similar. JSON format is text-only. The keys (unlike in JavaScript objects) are wrapped in quotes. JSON only contains primitive data types whereas in JavaScript objects, we can add functions as well.

```
{
 "firstName":"Melina", 
 "lastName":"Dorsey",
 “age”: 25
}
```

#### JSON objects
JSON objects are different from JSON. “JSON” is an in-built object (similar to console, window, etc) in JavaScript.

- JSON.parse()
  - Parsing means taking one format and transforming it into another. In JavaScript, we convert the data from JSON objects to JavaScript objects.
  - A function used to convert a string into a JavaScript object.
  ```
  let userDetails = '{"name":"Melina Dorsey","email":"melina.dorsey@example.com","age":25}';
  let userObj = JSON.parse(userDetails);
  ```
- JSON.stringify()
  - A function used to convert a JavaScript object into a string.
  ```
  let userDetails = {name: 'Melina Dorsey', email: 'melina.dorsey@example.com', age: 25};
  let userStr = JSON.stringify(userDetails);
  ```

The JSON string is used whenever we want to transfer data from one program to another, within the program, it is better to use the JavaScript object rather than using the string operations


### Supplemental Materials

- [JavaScript Objects](https://www.w3schools.com/js/js_objects.asp)
- [JSON](https://www.w3schools.com/js/js_json.asp)
- [Working with objects](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects)
- [Code.org video tutorial](https://www.youtube.com/watch?v=ZunUF_WGMb4)
- Work through [this interactive lesson on JavaScript Objects](https://www.codecademy.com/courses/introduction-to-javascript/lessons/objects/exercises/objects?action=resume_content_item)
- [Eloquent JavaScript, The Secret Life of Objects ](https://eloquentjavascript.net/06_object.html)
