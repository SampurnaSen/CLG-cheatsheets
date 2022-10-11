# Lesson 5 - Web APIs

### Projected Time

About 2 hours

### Lesson

#### APIs
Application Programming Interface. In the context of APIs, the word Application refers to any software with a distinct function. Interface can be thought of as a contract of service between two applications. This contract defines how the two communicate with each other using requests and responses.

Types of APIs:
- Browser APIs (Web APIs) - It can extend the functionality of a web browser. We’ll mainly focus on browser APIs in this lesson.
- Third Party APIs - built by a third party or by a backend developer and can be accessed only if we are allowed to.

#### Browser APIs
Built-in to your browser. You can use them to manipulate what your users see in their browser. You can also use them to fetch data or store data.

- Document API: The Document interface represents any web page loaded in the browser and serves as an entry point into the web page's content.
```
document //the main document object
document.body //returns the <body> node of the current document.
```
- Window API: Represents a browser window. Whenever a window appears on the screen to display the contents of a document, the window object is created. The document API is a child of the window API.
    - setTimeout(): calls a function after a number of milliseconds.
    ```
    function greet() {
        console.log('Hello world');
    }
    setTimeout(greet, 3000);
    console.log('This message is shown first');
    ```
    - setInterval(): calls a function at specified intervals (in milliseconds).
    - clearInterval(): used to stop the setInterval() call.
    - window.location: return set of details regarding the window you are on.
    - window.history: this object contains the browser's history.
        - history.back(): same as clicking back in the browser.
        - history.forward(): same as clicking forward in the browser.
    - localStorage: allows you to store some values in the browser. localStorage stores data with no expiration date. However, the user also could clear the browser data/cache to erase all local storage data.
        - setItem() - save the data  in local storage.
        - getItem() - read the data from local storage.
    - sessionStorage: allows you to store some values in the browser. sessionStorage stores data for one session (data is lost when the browser tab is closed).
        - setItem() - save the data  in local storage.
        - getItem() - read the data from local storage.


### Supplemental Materials

- [Web Storage](https://mdn.github.io/dom-examples/web-storage/)
- [Example: localStorage](https://www.w3schools.com/html/tryit.asp?filename=tryhtml5_webstorage_local_clickcount)
- [local vs session storage](https://www.xenonstack.com/insights/local-vs-session-storage-vs-cookie)