# Lesson 6 - Traversing DOM

### Projected Time

About 2 hours

### Lesson

#### The DOM
The DOM API targets the browser/web API and allows us to use CRUD operations to manipulate the HTML elements, styles and attributes. This means that the HTML document can be changed/modified to add elements, remove elements, edit elements, move elements around, etc.

CRUD: is an acronym for create, read, update and delete. We usually use this term in backend development. It’s basically manipulating your data.

#### The DOM Node Tree
We read the element in our HTML document as nodes within a tree structure. Various things that are nodes are the document itself, elements, text, and comments. Top node/root node is the document object, followed by the <head>, <body> as children.

#### Manipulating the DOM
- style: We can change the style property . [Similar to CSS styles but in camelCase]
```
document.body.style.backgroundColor = “pink”;
```
- innerHTML: changes the inner content of HTML.
```
document.body.innerHTML = "Hello"
```
- getElementByID: used to get an element with that ID.
```
document.getElementById("content");
document.getElementById("content").style.color = “pink”;
```
- querySelector: selects the FIRST element on the page that fits the query.
```
document.querySelector(‘p’);
document.querySelector(‘p’).style.color = “pink”;
```
- classList: returns classes assigned to the specific element. Has methods like `add()`, `remove()`, `toggle()`
```
document.getElementById("content").classList;
document.getElementById("content").classList.add("test-class");
```
- addEventListener: attaches an event handler to an element.
```
document.getElementById("myBtn").addEventListener("click", changeColor);
function changeColor() {
  document.querySelector(‘p’).style.color = “pink”;
}
```

Events can be categorized in many ways. Some are:
- Mouse events
  - click
  - contextmenu : right click `.addEventListener("contextmenu", myFun());`
  - dblclick: double click
  - mouseover/mouseout
  - mousemove
- Keyboard events
  - keydown & keyup
  - keypress

We can also apply events to our HTML elements using the “on” listener:
- onClick(): `<button onclick="clickMe()"> CLICK ME </button>`
- onChange(): used when the value changes (dropdowns)
- onFocus(): `<input type="text" onfocus="highlightInput(this)">`


### Supplemental Materials

- [DOM tree viewer](https://software.hixie.ch/utilities/js/live-dom-viewer/)
- [What is DOM?](https://www.freecodecamp.org/news/whats-the-document-object-model-and-why-you-should-know-how-to-use-it-1a2d0bc5429d/)
- [DOM manipulation](https://www.freecodecamp.org/news/dom-manipulation-in-vanilla-js-2036a568dcd9/)
- [EventListener examples](https://www.javatpoint.com/javascript-addeventlistener)