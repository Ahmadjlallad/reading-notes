#### Design web pages with CSS
* CSS: (Cascading Style Sheets) allows you to create great-looking web pages, is a language for specifying how documents are presented to users — how they are styled.
* CSS syntax: ```h1 {color: red; font-size: 5em;}``` ```h1```  selector rule opens with it, in Inside ```{ }``` will be one or more declarations, ```color``` here called property, ```red``` is the value.
* CSS Specifications: All web standards technologies (HTML, CSS, JavaScript, etc.) are defined in giant documents called specifications (or "specs"), which are published by standards organizations (such as the W3C, WHATWG, ECMA, or Khronos) and define precisely how those technologies are supposed to behave.
  * As a newcomer to CSS, it is likely that you will find the CSS specs overwhelming — they are intended for engineers to use to implement support for the features in user agents, not for web developers to read to understand CSS.
* How To Add CSS: 
  * External CSS
  * Internal CSS
  * Inline CSS
  1. External CSS:you can change the look of an entire website by changing just one file!
    * HTML must include a reference to the external style sheet file inside the ```<link>``` element, inside the head section```<link rel="stylesheet" href="mystyle.css">```, .css file should not contain any HTML tags.
  2. Internal CSS: one single HTML page has a unique style. The internal style is defined inside the ```<style>``` element, inside the head section.
  3. Inline CSS: An inline style may be used to apply a unique style for a single element.
* Multiple Style Sheets: If some properties have been defined for the same selector (element) in different style sheetsd. 
  * if you define internal style after inked external style the element will be styled as internal style and vice versa
* Cascading Order: more than one style specified for an HTML element
  * where alphabet a has the highest priority:
    1. Inline style
    1. External and internal style sheets 
    1. Browser default










