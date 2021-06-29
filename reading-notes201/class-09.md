# HTML

- Traditionally, the term 'form' has referred to a printed document that contains spaces for you to fill in information.

- HTML borrows the concept of a form to refer to different elements that allow you to collect information from visitors to your site.

- how Forms Work
  - The name of each form control is sent to the server along with the value the user enters or selects.
  - The server processes the information using a programming language such as PHP, C#, VB.net, or Java. It may also store the information in a database.
  - The server creates a new page to send back to the browser based on the information received.

### Multiple Style Sheets

- `<form>`form controls live inside a `<form>` element.
  - `action` attributes Every <form> element requires an action attribute. Its value is the URL for the page on the server that will receive the information in the form when it is submitted.
  - `method` attributesForms can be sent using one of two methods: get or post.
- Text Input `<input>` element is used to create several different form controls.

  - `type="text"` it creates a single line text input.
    - `name`each form control requires a name attribute. The value of this attribute identifies the form control and is sent along with the information they enter to the server.
    - `maxlength` You can use the maxlength attribute to limit the number of characters a user may enter into the text field.

- PassWord input `type="password"` When the type attribute hasa value of password it creates a text box that acts just like a single-line text input, except the characters are blocked out. They are hidden in this way so that if someone is looking over the user's shoulder, they cannot see sensitive data such as passwords.
- Text Area `<textarea>`The element is used to create a mutli-line text input.
- Radio button `type="radio"` Radio buttons allow users to pick
  just one of a number of options.
  - `value`attribute indicates the value that is sent to the server for the selected option.
  - `checked` attribute can be used to indicate which value (if any) should be selected when the page loads.
- CheckBox `type="checkbox"` Checkboxes allow users to select (and unselect) one or more options in answer to a question, name, value, checked same as before.
- Drop down list box `<select>` A drop down list box (also known as a select box) allows users to select one option from a drop down list.
- `<option>`The `<option>` element is used to specify the options that the user can select from. The words between the opening `<option>` and closing `</option>` tags will be shown to the user in the drop down box

```HTML
<select name="devices">
<option value="ipod">iPod</option>
<option value="radio">Radio</option>
<option value="computer">Computer</option>
</select>
```

`multiple` You can allow users to select multiple options from this list by adding the multiple attribute with a value of multiple.

- File input box `<input>` If you want to allow users to upload a file (for example an image, video, mp3, or a PDF), you will need to use a file input box.
  - `type="file"` creates a box text input followed by a browse button user clicks on the browse button, a window opens up that allows them to select a file from their computer to be uploaded to the website.
- Submit Button `<input type="submit">`
- Image Button `<input type="image">` The src, width, height, and alt attributes work just like they do when used with the `<img>` element
- button & hidden controls `<button>`This means that you can combine text and images between the opening `<button>` tag and closing `</button> `tag. `<input>` type="hidden"They allow web page authors to add values to forms that users cannot see.
- `<label>` \* Wrap around both the text description and the form input, Be kept separate from the form control and use the for attribute to indicate which form control it is a label `for`.
- grouping form elements `<fieldset>` ou can group related form controls together inside the `<fieldset>` element.
- `<legend>` The `<legend>` element can come directly after the opening `<fieldset>` tag and contains a caption which helps identify the purpose of that group of form controls.

- html5: form validation web that give users messages if the form control has not been filled in correctly; this is known as form validation.

# CSS

#### list-style-type

- property allows you to control the shape or style of a bullet point.
- list-style-image specify an image to act as a bullet point using the list-style-image property
- list-style-position `outside`The marker sits to the left of the block of text, `inside`The marker sits inside the box of
  text (which is indented).
- `list-style` shorthand property

#### Table Properties

- same as we learned before

- `border-spacing`, `border-collapse`

- The border-spacing property allows you to control the distance between adjacent cells. By default, browsers often leave a small gap between each table cell, so if you want to increase or decrease this space then
  the border-spacing property allows you to control the gap Chapter.

- `collapse` Borders are collapsed into a single border where possible.
- `separate` Borders are detached from each other.

#### styLing Forms

Styling Text Inputs

- The `:focus` pseudo-class is used to change the background color of the text input when it is being used, and the `:hover` pseudo-class applies the same styles when the user hovers over them.

- The `cursor` property allows you to control the type of mouse cursor that should be displayed to users.

# JS

#### DIFFERENT EVENT TYPES

selection of the events that occur in the browser while you are browsing the web. Any of these events can be used to trigger a function in your JavaScript code.

EVENT DESCRIPTION
UI EVENTS

- load W eb page has finished loading
- unload Web page is unloading (usually because a new page was requested)
- error Browser encounters a JavaScript error or an asset doesn't exist
- resize Browser window has been resized
- scroll User has scrolled up or down the page
  KEYBOARD EVENTS
- keydown User first presses a key (repeats while key is depressed)
- keyup User releases a key
- keypress Character is being inserted (repeats while key is depressed)

- click User presses and releases a button over the same element
- dbl click User presses and releases a button twice over the same element
- mouse down User presses a mouse button while over an element
- mouse up User releases a mouse button while over an element
- mouse move User moves the mouse (not on a touchscreen)
- mouse over User moves the mouse over an element (not on a touchscreen)
- mouse out User moves the mouse off an element (not on a touchscreen)

#### HOW EVENTS TRIGGER JAVASCRIPT CODE

When the user interacts with the HTML on a web page, there are three
steps involved in getting it to trigger some JavaScript code.
Together these steps are known as event handling.

- Select t he element node(s) you want the script to respond to
  -Indicate which event on the selected node(s) will trigger the response.
- State the code you want to run when the event occurs.

### THREE WAYS TO BIND AN EVENT TO AN ELEM ENT

- HTML EVENT HANDLERS **_bad practice_**
- TRADITIONAL DOM EVENT HANDLERS let you separate the JavaScript from the HTML

  - The main drawback is that you can only attach a single function to any event. sold but not good Enough

- DOM LEVEL 2 EVENT LISTENERS were introduced in an update to the DOM
  specification hese newer event listeners allow one event to trigger multiple functions. As a result, there are less likely to be conflicts
  between different scripts that run on the same page

js`element .addEventlistener('event', functionName [, Boolean]) `

The addEventli stener() method takes three properties:

- The event you want it to listen for.
- The code that you want it to run when the event fires

#### USING PARAMETERS WITHEVENT HANDLERS & LISTENERS

- you wrap the function call in an anonymous function

```js
elUsername.addEventListener(
  "blur",
  function () {
    checkUsername(S);
  },
  false
);
```

#### Event Flow

- When you click an element that is nested in various other elements, before your click actually reaches its destination, or target element , it must trigger the click event each of its parent elements first, starting at the top with the global window object.

- useCapture is false. So basically it decides whether the event is handled in the capture or the bubble phase of event processing. As long as no of the element's parents (or children) have any similar events attached, there is no real difference

#### THE EVENT OBJECT

- event listener's event occurs and it calls its associated function, it also passes a single argument to the function—a reference to the event object. The event object contains a number of properties that describe the event that occurred.
