# Basics of HTML, CSS & JS

## Text

* Headings

```#!HTML
<h1>This is a Main Heading</h1>
<h2>This is a Level 2 Heading</h2>
<h3>This is a Level 3 Heading</h3>
<h4>This is a Level 4 Heading</h4>
<h5>This is a Level 5 Heading</h5>
<h6>This is a Level 6 Heading</h6>
```


| tag      | uses |
| ---------| -----|
| Bold  ```<b>``` | make characters appear bold.| 
| ITalic ```<i>```| make characters appear italic.|
|Superscript ```<sup>```|raising a number to a power 2<sup>2</sup>|
|Subscript ```<sub>```|H<sub>2</sub>O|
|Line Break ```<br />```|add a line break.|
|horizontal rule ```<hr />```| create a break between tham|
|```<strong>```|indicates that its content has strong importance.|
|```<em>```|emphasis that subtly changes the meaning of a sentence.|
|```<blockquote>```| element isused for longer quotes that take up an entire paragraph.|
|```<q>```|shorter quotes|
|```<abbr>```|abbreviation or an acronym <abbr title="abbreviation or an acronym">exmple</abbe>|
|```<cite>```| used to indicate where the citation is from.|
|```<dfn>```|indicate the defining instance of a new term.|
|```<ins> <del>```|show content that has been inserted into a document, show text that has been deleted from it.|
|```<s>```|indicates something that is no longer accurate or relevant (but that should not be deleted)|

## Introducing CSS

```#!CSS
selector {
<!--declaration-->
<!--proprty = value  -->
    color   = red;
}
```

* A CSS selector is the first part of a CSS Rule. It is a pattern of elements and other terms that tell the browser which HTML elements should be selected to have the CSS property values inside the rule applied to them.
  * Internal or embedded:add ```<style>``` tag in the ```<head>``` section of HTML document
  * External:link the HTML sheet to a separate .css file
  * Inline:apply CSS rules for specific elements.
* alows use Internal

|selectors|example|
|--------|---------|
|universaL SeLector|```* {}``` Targets all elements on the page|
|class Selector|```.note {}``` Targets any element whose class attribute has a value of note|
|type Selector|```h1, h2, h3 {}``` Targets the ```<h1>```, ```<h2>``` and ```<h3>```elements|
|Id Selector|```#introduction {}```|
|descendant Selector|```p a {}```|

* Inheritance: inheritance controls what happens when no value is specified for a property on an element.
  * CSS properties can be categorized in two types:
    * inherited properties, which by default are set to the computed value of the parent element for example ```color```.
    * non-inherited properties, which by default are set to initial value of the property ```border```.

## JavaScript

### Basic JavaScript Instructions

* **statement**: A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a **statement** js is *case sensitive*.

* **DATA TYPES**

|DATA|TYPE|
|--------|--------|
|0-9|**NUMERIC**,The numeric data type handles numbers|
|**'** ahmad **'**|**STRING** enclosed within a pair of quotes.|
|true, falus|BOOLEAN|

* **Storing** using variable ```let ahmad = 'jallad'``` now ```ahmad``` store ```jallad```straing  alsow ```let ahmad = 20``` storing number maybe you want to store boolen ok ```let ahmad = true``` lovely.
 
* **ARRAYS**:  is a single variable that is used to store different elements. It is often used when we want to store list of elements and access them by a single variable.
```let vegetables = ['Cabbage', 'Turnip', 'Radish', 'Carrot']```
```let my_fav_vegetables = vegetables[3]```this is mean my_fav_vegetables =```Carrot```

### Decisions and Loops

* **COMPARISON** OPERATORS

At the most basic level, you can evaluate two variables using a comparison operator to return at true or false value.```var hasPassed = score >= pass ;```

* **LOGICAL** OPERATORS

|Name|Symbol|
|--------|--------|
|AND|```&& (scorel >= passl) && (score2 >= pass2);```|
|OR|```|| (scorel >= passl) || (score2 >= pass2);```|
|NOT|```!(true)```|

* **IF** STATEMENTS

```#!html
if (condition1) {
  //  block of code to be executed if condition1 is true
} else if (condition2) {
  //  block of code to be executed if the condition1 is false and condition2 is true
} else {
  //  block of code to be executed if the condition1 is false and condition2 is false
}
```

* **SWITCH** STATEMENTS
  * Use the switch statement to select one of many code blocks to be executed.
  * The switch statement is used to perform different actions based on different conditions.

```#!html
switch(expression) {
  case x:
    // code block
    break;
  case y:
    // code block
    break;
  default:
    // code block
}
```