# Read: 06 - JS Object Literals; The DOM
# Understanding The Problem Domain:
* Create a familiar problem domain because it is very difficult to learn more than one thing at once.
* Make the problem domain easier by cutting out cases and narrowing your focus to a particular part of the problem.
* Get better at understanding the problem domain, It is much more expensive and time consuming to do things over than it is to do them right the first time.

# Object Literals in JavaScript:
## What is an Object?
* Objects group together a set of variables and functions to create a model of a something you would recognize from the real world.
 * In an object: variables become known as **Properties**.
 * In an object: functions become known as **Methods**.
* An Example of an object:
``` var hotel = {
    name : 'Quay';
    rooms: 4;
    gym: true;
    checkAvailable: function(){
        do this;
    }
}
```

* Accessing the object using dot notaion or square brackets.
![](https://raw.githubusercontent.com/ATL-WDI-Curriculum/js-objects-and-json/master/images/object-property-method.jpg)


# Document Object Model (DOM):
* The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.
* The DOM is neither part of HTML, nor part of JavaScript; it is a separate set of rules.
* The DOM is called an object model because the model is made of objects.
* Each object represents a different part of the page loaded in the browser window.

## DOM tree:
* As a browser loads a web page, it creates a model of that page. The model is called a DOM tree, and it is stored in the browsers' memory.
* It consists of four main types of nodes, Every element, attribute, and piece of text in the HTML is represented by its own DOM node.
 1. **The Document node**: At the top of the tree a document node is added; it represents the entire page,It is the starting point for all visits to the DOM tree.
 2. **Elements node**: To access the DOM tree, you start by looking for elements. Once you find the element you want, then you can access its text and attribute nodes if you want to.
 4. **Attribute nodes**: are not children of the element that carries them; they are part of that element.
 5. **Text nodes**: Once you have accessed an element node, you can then reach the text within that element. This is stored in its own text node.

 ![](https://raw.githubusercontent.com/10Pines/ghost-storage/master/2018/08/Arbol.png)

## DOM Queries:
* They are methods who finds elements in the DOM tree.
* DOM queries may return one element, or they may return a Nodelist, which is a collection of nodes.
* Methods that return one element:
  * `getElementByld(id) ` : allows you to select a single element node by specifying the value of its id attribute.
  * `querySelector(css selector)`: take a CSS selector as their only parameter.
  * `getElementsByClassName(class)`: allows you to select elements whose css attribute contains a specific value.
  * `getElementsByTagName(tagName)`: allows you to select elements using their tag name.
  * `querySelectorAll (css selector)`: take a CSS selector as their only parameter.
* Methods that return more than one element:
 * `getElementsByTagName(tagName)`
 * `getElementsByClassName(class)`
 * `querySelectorAll (css selector)`

## Looping through a nodelist:
* Example:
``` var hotItems = document.querySelectorAll('li.hot');
if (hotltems.length > O) {
    for (var i=O; i<hotl tems.length; i++){
        hotltems[i].className = 'cool';
    }
 ```

## Accesse and update text and markup:
* Using the **innerHTML property**, you can access and amend the contents of an element, including any child elements.

## Adding an element using DOM manipulation:
1. Create the element: `createElement()`
2. Give it content: `createTextNode()`
3. Add it to the DOM: `appendChild()`

## Removing an element using DOM manipuation:
1. Store the element to be remove in a variable.
2. Store its parent in a variable.
3. Remove the element from its containing element: `removeChild()`.

![](https://www.kirupa.com/html5/images/DOM_js_72.png)