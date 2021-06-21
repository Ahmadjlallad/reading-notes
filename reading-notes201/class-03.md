# HTML

## *Lists*

### Order list

* **Ordered** HTML List ```<ol>``` as to create order list Each list item starts with the ```<li>``` tag The list items will be marked with numbers by default.

```#!html
<ol>
    <li>Fasten your seatbelt</li>
    <li>Starts the car's engine</li>
    <li>Look around and go</li>
</ol>
```

* **Unordered** List ```<ul>``` Each list item starts with the ```<li>``` tag.
The list items will be marked with bullets.

```#!html
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```

* **Definition** The ```<dl>``` tag is used in conjunction with ```<dt>``` (defines terms/names) and ```<dd>``` (describes each term/name).

```#!html
<dl>
  <dt>Coffee</dt>
  <dd>Black hot drink</dd>
  <dt>Milk</dt>
  <dd>White cold drink</dd>
</dl>
```

example

<dl>
  <dt>Coffee</dt>
  <dd>Black hot drink</dd>
  <dt>Milk</dt>
  <dd>White cold drink</dd>
</dl>

* * *

# CSS

## *Boxes*

### Box Dimensions

* width, height
  * By default, the width and height of an element is calculated like this: width + padding + border = actual width of an element, height + padding + border = actual height of an element.(w3s)

  * limiting width
   ```min-width, max-width``` min-width property specifiesthe smallest size a box can bedisplayed at when the browser window is narrow, and the max-width property indicates the maximum width a box can stretch to when the browser window is wide.(same for ```min-height, max-height``` )

  * Overflowing content Everything in CSS is a box. You can constrain the size of these boxes by assigning values of width and height (or inline-size and block-size). Overflow happens when there is too much content to fit in a box.(Mdn)
    * hidden This property simply hides any extra content that does not fit in the box.
    * scroll This property adds a scrollbar to the box so that users can scroll to see the missing content.

```#!css  
p.one {
overflow: hidden;
overflow: scroll;}
}
```

* border margin padding
  * Content - The content of the box, where text and images appear.
  * Padding - Clears an area around the content. The padding is transparent.
  * Border - A border that goes around the padding and content.
  * Margin - Clears an area outside the border. The margin is transparent.
![border margin padding](https://www.w3.org/Style/css2-updates/css2/images/boxdim.png).(W3)

* Border
  * border-width
    * medium Specifies a medium border. This is default
    * thin Specifies a thin border
    * thick Specifies a thick border
    * length Allows you to define the thickness of the border. Read about length units

  * border-style
    * solid
    * dashed
    * hidden / none
    * dotted
  * border-color You can specify the color of a border.

* Padding
  * The padding property allows you to specify how much space should appear between the content of an element and its border.

* Margin The margin property controls the gap between boxes.

* display Property
  * inline Displays an element as an inline element (like ```<span>```). Any height and width properties will have no effect.(w3s)
  * block Displays an element as a block element (like ```<p>```). It starts on a new line, and takes up the whole width.(w3s)
  * inline-block Displays an element as an inline-level block container. The element itself is formatted as an inline element, but you can apply height and width values.(w3s)
* visibility
  * hidden This hides the element.
  * visible This shows the element.
* border-image The border-image property applies an image to the border of any box.
  * **stretch** stretches the image
  * **repeat** repeats the image
  * **round** like repeat but if the tiles do not fit exactly, scales the tile image so they will
* border-radius
  * To create more complex shapes

* * *

# JS

182

* Truthy and falsy
  * The following values are always falsy:
    * ```false```
    * ```0 (zero)```
    * ```'' or "" (empty string)```
    * ```null```
    * ```undefined```
    * ```NaN```
  * Everything else is truthy.

|```==```|```true```|```false```|```0```|```''```|```null```|```undefined```|```NaN```|```Infinity```|```[]```|```{}```|
|-|-|-|-|-|-|-|-|-|-|-|
|```true```|true| false| false| false| false| false| false| false| false| false|
|```false```|false|true|true|true|false|false|false|false|true|false|
|```0```|false| true| true| true| false| false| false| false| true| false|
|```''```|false| true| true |true |false |false |false| false |true| false|
|```null```|false |false |false |false |true| true |false |false |false| false|
|```undefined```|false |false |false |false| true |true |false| false |false |false|
|```NaN```|false |false |false |false |false |false |false |false |false |false|
|```Infinity```|false |false |false |false |false |false |false|true|false|false|
|```[]```|false |true |true|true|false|false|false|false|false|false|
|```{}```|false |false|false|false|false|false|false |alse |false|false|false|

## Loops

### KEY LOOP CONCEPTS

* break This keyword causes the termination of the loop and tells the interpreter to go onto the next statement of code outside of the loop. (You may also see it used in functions.)

* continue
This keyword tells the interpreter to continue with the current iteration, and then check the condition again. (If it is true, the code runs again.

* USING FOR LOOPS The for statement creates a loop that consists of three optional expressions, enclosed in parentheses and separated by semicolons, followed by a statement (usually a block statement) to be executed in the loop.

```js
for ([initialization]; [condition]; [final-expression])
   statement
```