# Problem Domain, Objects, and the DOM

## Problem Domain.

is hard because you can’t really see what you are trying to build very clearly.

> The real world is a messy place. Many of the problem domains we face as programmers are difficult to understand and look completely different depending on your viewpoint.
> John Sonmez

Programming is easy if you understand the problem domain

- Make the problem domain easier
- Get better at understanding the problem domain
  _You can often make the problem domain easier by cutting out cases and narrowing your focus to a particular part of the problem_
  but be careful It is easy to fall into the trap of thinking you understand enough of the problem to get started coding it.

# JS

## OBJECT

**a set of variables and functions to create a model of a something you would recognize from the real world.**
**variables become known as properties**

- variables become known as properties
- properties and methods have a name and a value. In an object, that name is called a key
  - An object cannot have two keys with the same name.

creating an object:

```js
const person = {
  firstName: "John",
  lastName: "Doe",
  age: 50,
  eyeColor: "blue",
};
person["lastName"];
```

access object/Dot notation
`objectName.propertyName objectName["propertyName"]`

## DOM

how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.
A **DOM** **_tree_** starts from the topmost element which is html element and branches out as per the occurrence and nesting of HTML elements in the document.
![Dom tree](https://www.researchgate.net/profile/Olfa-Nasraoui/publication/221417012/figure/fig2/AS:669043992322053@1536523926785/Dom-Tree-of-An-Example-Web-Page.png)

- it creates a model of that page and it is stored in the browsers' memory.It consists of four main types of nodes.

---

- ACCESS THE ELEMENTS

  - `getElementByld ()` id attribute
  - `querySe1ector()` Uses a CSS selector, and returns the first matching element

- SELECT MULTIPLE ELEMENTS

  - `getElementsByClassName()`
  - `getElementsByTagName()`
  - `querySelectorAll()`

---

- WORK WITH THOSE ELEMENTS
  - access/ update text nodes
    - Select the `<li>`element
    - Use the first Child property to get the text node
    - Use the text node's only property (nodeValue) to get the text from the element
  - WORK WITH HTML CONTENT
    - `createElement(), createTextNode()`
  - ACCESS OR UPDATE ATTRIBUTE VALUES
    - `hasAttribute(), getAttribute(), setAttribute() ,removeAttribute()`

---

- selecting an element from a NodeList
  - item() METHOD `document.getElementsByClassName('hot').item(0)`
  - Array Index `document.getElementsByClassName('hot')[0]`

---

- Previous & next sibling

  - `.nextSibling`return next in the tree.
  - `.previousSibling;` return previous in the tree.

- first & last child

  - `.firstchild`will return the first element
  - `.lastchild` will return the last element

- `.nodeValue` retrieve or amend the content of it using the nodeVa1ue property.

- `.replace` change the contact in it

- `.textContent()` allows you to collect or update just the text that is in the containing element

  (pp.183-242)
