# Readings Notes for Class 3

## HTML

### Links

<div style="position: fixed;
  bottom: 0;
  right: 0;
  width: 300px;
  border: 3px solid #73AD21;">This &lt div &gt element has position: fixed;(W3s)</div>

* An ```<a>``` anchor tag is a HTML element that creates a link to a target URL. When correctly implemented, the link can wrap around text, images, or as buttons, so that users can interact with it and visit the link's destination.
  * Linking to other sites Example From W3s.
  * Linking to other pages on the same site.
  * link to paragraph in the same page.

```html
<a href="https://www.w3schools.com" target="_blank">Visit W3Schools.com!</a>
```

* 
  * ```target="_blank"``` Specifies where to open the linked document in case of ```_blank``` open in a new tap.

### Dealing with files(Mdn)

* What structure should your website have?

1. index.html: This file will generally contain your homepage content, that is, the text and images that people see when they first go to your site. Using your text editor, create a new file called index.html and save it just inside your test-site folder.
1. images folder: This folder will contain all the images that you use on your site. Create a folder called images, inside your test-site folder.
1. styles folder: This folder will contain the CSS code used to style your content (for example, setting text and background colors). Create a folder called styles, inside your test-site folder.
1. scripts folder: This folder will contain all the JavaScript code used to add interactive functionality to your site (e.g. buttons that load data when clicked). Create a folder called scripts, inside your test-site folder.
(tree style)

* * * 

## CSS

### Layout

* First learn to crate a right element either be a block or inline block.
* containing ElEmEnts If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.
* ControLLing the position of eLements:
  * Normal flow.```position:static```
  * Relative Positioning:is positioned relative to its normal position. shifting it to the top, right,bottom, or left of where it would have been placed. This does not affect the position of surrounding elements```position:relative```
  * Absolute Positioning: This positions the element in relation to its containing element.
  * ```position:fixed``` is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled. The top, right, bottom, and left properties are used to position the element.W3s
  * The z-index property specifies the stack order of an element.
    * An element with greater stack order is always in front of an element with a lower stack order.```z-index: 10;```boxes can overlap. If boxes do overlap, the elements that appear later in theHTML code sit on top of those that are earlier in the page.

* * *

## JS

### FUNCTION: let you group a series of statements together to perform a specific task.

declaration

```js
function square(number) {
  return number * number;
}
```

takes one parameter, called number.
```return```

* The statement return specifies the value returned by the function ether single value or multiple using arrays

### Declaration & Call

* the interpreter alwayslooks for variables and function declarations before going through each section of a script, line-by-line.This means that a function created with a function declaration can be called before it has even been declared.

* declared as above 
* Declared function expression name is usually omitted meaning its anonymous function.
  * function is not processed until the interpreter gets to that statement. This means you cannot call this function before the interpreter has discovered it. It also means that any code that appears up to that point could potentially alter what goes on inside this function.
anonymous, For example(Mdn)

```js
const square = function(number) { return number * number }
var x = square(4) // x gets the value 16
```

* IMMEDIATELY INVOKED FUNCTION EXPRESSIONS
  * hey are used for code that only needs to run once within a task, rather than repeatedly being called by other parts of the script.
  * to calculate a value for that function
  * to calculate a value for that function
  * To prevent conflicts between two scripts that might use the same variable names

### VARIABLE SCOPE

* The location where you declare a variable will affect where it can be used within your code. If you declare it within a function, it can only be used within that function. This is known as the variable's scope.
  * LOCAL VARIABLES: function-level scope. It cannot be accessed outside of the function.
    * The interpreter creates local variables when the function is run, and removes them as soon as the function has finished its task. 
    * If the function runs twice, the variable can have different values each time
    * Two different functions can use variables with the same name without any kind of naming conflict.

* GLOBAL VARIABLES any variables created outside or in the main scope.
  * Global variables are stored in memory for as long as the web page is loaded into the web browser.

