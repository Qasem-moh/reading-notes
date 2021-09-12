# Component Based UI(user interface)
* JSX is an extension of the JavaScript language based on ES6, and is translated into regular JavaScript at runtime. 
* JSX stands for JavaScript XML.
* JSX allows us to write HTML elements in JavaScript and place them in the DOM without any createElement()  and/or appendChild() methods.
* JSX converts HTML tags into react elements. ``const element = <h1>Hello, world!</h1>;``
* React is a JavaScript library
* Benefits OF JSX:
    1. it helpful as a visual aid when working with UI inside the JavaScript code.
    2. It also allows React to show more useful error and warning messages.
* You can put any valid JavaScript expression inside the curly braces in JSX.
``const element = (``

```<h1>```

   `` Hello, {formatName(user)}!``

  ``</h1>``
``);``

``ReactDOM.render(``

 `` element,``

 `` document.getElementById('root')``
``);``

* We can use JSX inside of if statements and for loops, assign it to variables, accept it as arguments, and return it from functions
* You can either use quotes (for string values) or curly braces (for expressions), but not both in the same attribute
* If a tag is empty, you may close it immediately with />, like XML ``const element = <img src={user.avatarUrl} />;``
* JSX tags may contain children
* It is safe to embed user input in JSX; so JSX Prevents Injection Attacks 
``const title = response.potentiallyMaliciousInput;``

``const element = <h1>{title}</h1>;``

* React.createElement() performs a few checks to help you write bug-free code but essentially it creates an object called React elements

``const element = {``

``type: 'h1',``

``props: {``

``className: 'greeting',``

``children: 'Hello, world!'``
``}``
``};``

* Applications built with just React usually have a single root DOM node. If you are integrating React into an existing app, you may have as many isolated root DOM nodes as you like.
* React elements are immutable. Once you create an element, you can’t change its children or attributes.
* With our knowledge so far, the only way to update the UI is to create a new element, and pass it to ReactDOM.render``().`` React Only Updates What’s Necessary


# Term
* **Rendering** : generates the visual output for the user
* **template** is HTML markup, peppered with tags that will either insert variables or run programming logic
* **State** describes the status of the entire program or an individual object. It could be text, a number, a boolean, or another data type. It's a common tool for coordinating code.


# Q
1. Name 5 Javascript UI Frameworks (other than React)
    * Angular
    * Webix
    * Vue
    * Sencha
    * SolidJS
2. What’s the difference between a framework and a library?
- The technical difference between a framework and library lies in a term called inversion of control. When you use a library, you are in charge of the flow of the application. You are choosing when and where to call the library. When you use a framework, the framework is in charge of the flow

![check](https://anarsolutions.com/wp-content/uploads/2019/02/Library-and-Framework.jpg)