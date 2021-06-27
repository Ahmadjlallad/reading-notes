# Object-Oriented Programming, HTML Tables

## HTML

### Tables

#### A table represents information in a grid format

- table structure

```html
<table>
  <thead>
    <tr>
      <th>15</th>
      <th>15</th>
      <th>30</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>45</th>
      <td>60</td>
      <td>45</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <th>60</th>
      <td>90</td>
      <td>90</td>
    </tr>
  </tfoot>
</table>
```

- `<table>`element is used to create a table.
- `<tr>` You indicate the start of each row, The tr stands for table row.
- `<td>`Each cell of a table is represented, The td stands for
  table data
- `<th>`purpose is to represent the heading for either a column or
  a row, table heading, helps people who use screen readers, improves the ability for search engines
  to index your pages, and also enables you to control the appearance of tables better when you start to use css.
- colspan attribute can be used on a `<th>` or `<td>` element and indicates how many columns that cell should run across
  `<td colspan="2">Geography</td>`

- `<thead>`The headings of the table should sit inside the `<thead>` element.
- **long Tables**
- `<tbody>`The body should sit inside the
- `<tbody>` element.
- `<tfoot>`The footer belongs inside the
  `<tfoot>` element

## JS

### Object-Oriented Programming

#### Constructor Notation

creating objects using constructor syntax
Sometimes we need a "blueprint" for creating many objects of the same "type".
The way to create an "object type", is to use an object constructor function.

- Example from W3s

```js
function Person(first, last, age, eye) {
  this.firstName = first;
  this.lastName = last;
  this.age = age;
  this.eyeColor = eye;
}
```

Objects of the same type are created by calling the constructor function with the `new` keyword:

- Example from W3s

```js
const myFather = new Person("John", "Doe", 50, "blue");
const myMother = new Person("Sally", "Rally", 48, "green");
```

you can ues `delete`, `delete myFather.firstName;`

<br>

- what are built-in objects? a set of built-in objects that represent things like the browser window and the current web page shown in that window. These built-in objects act like a toolkit for creating interactive web pages, has three compartments:

- The Browser Object Model contains objects that represent the current browser window or tab.
- DOCUMENT OBJECT MODEL create a representation of
  the current page.**_THE WINDOW OBJECT_**
- The global JavaScript objects represent things that the JavaScript language needs to create a model
  of.

**THE WINDOW OBJECT**
represents the current browser window or tab.

`window.innerHeight`Height of window (excluding browser chrome/user interface) (in pixels)
`window.innerWidth`Width of window (excluding browser chrome/user
interface) (in pixels)
`window.a1ert()` Creates dialog box with message

---

- global objects:string object
  |Function|Description|
  |-|-|
  |`charAt()`|Returns the character at the specified index (position)|
  |`toLowerCase()`|Converts a string to lowercase letters|
  |`toString()` |Returns the value of a String object|
  |`toUpperCase()` |Converts a string to uppercase letters|
  |`trim()` |Removes whitespace from both ends of a string|
  |`endsWith()` |Checks whether a string ends with specified string characters|
  |`search()`| Searches a string for a specified value, or regular expression, and returns the position of the match|
  |`lastIndexOf()`| Returns the position of the last found occurrence of a specified value in a string|

---

- global objects:number object
  |Function|Description|
  |-|-|
  |`isNaN()`|Determines whether a value is an illegal number|
  |`parseFloat()`|Parses a string and returns a floating point number|
  |`parseInt()`|Parses a string and returns an integer|
  |`String()`| Converts an object's value to a string|
- global objects:Math Object
  - `Math.PI` Returns pi.
    |Function|Description|
    |-|-|
    |`Math.round(x)`| Returns x rounded to its nearest integer|
    |`Math.ceil(x)` |Returns x rounded up to its nearest integer|
    |`Math.floor(x)`| Returns x rounded down to its nearest integer|
    |`Math.trunc(x)`| Returns the integer part of x (new in ES6)|
    |`Math. random()`|Generates a random number between 0 (inclusive) and 1(not inclusive)|

---

- Global objects:Date Objects
  By default, JavaScript will use the browser's time zone and display a date as a full text
  **Creating** Date Objects
  Date objects are created with the `new` Date() constructor

```js
new Date()
new Date(year, month, day, hours, minutes, seconds, milliseconds)
new Date(milliseconds)
new Date(date string)
```

| Function                      | Description                                      |
| ----------------------------- | ------------------------------------------------ |
| `getDate() setDate()`         | Returns / sets the day of the month              |
| `getDay ()`                   | Returns the day of the week                      |
| `getFullYear() setFullYear()` | Returns / sets the year                          |
| `getHours () setHours ()`     | ReturnsI sets the hour                           |
| `getMinutes () setMinutes ()` | Returns / sets the minutes                       |
| `getSeconds() setSeconds()`   | Returns / sets the seconds                       |
| `toDateString ()`             | Returns "date" as a human-readable string        |
| `toTimeString ()`             | Returns "time" as a human-readable string        |
| `toString()`                  | Returns a string representing the specified date |
