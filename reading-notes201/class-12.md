# Chart.js & Canvas

### Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.

- JavaScript plugin that uses HTML5’s canvas element, makes using all kinds of bar charts, line charts, pie charts and more, incredibly easy.

- in the head element `<script src='Chart.min.js'></script>`

- Drawing a line chart

```html
<canvas id="buyers" width="600" height="400"></canvas>
```

```js
new Chart(buyers).Line(buyerData);
```

making object Data That will display

```js
var buyerData = {
  labels: ["January", "February", "March", "April", "May", "June"],
  datasets: [
    {
      fillColor: "rgba(172,194,132,0.4)",
      strokeColor: "#ACC26D",
      pointColor: "#fff",
      pointStrokeColor: "#9DB86D",
      data: [203, 156, 99, 251, 305, 247],
    },
  ],
};
```

- Drawing a pie chart

`<canvas id="countries" width="600" height="400"></canvas>` same as line chart

```js
var countries = document.getElementById("countries").getContext("2d");
new Chart(countries).Pie(pieData, pieOptions);
```

```js
var pieData = [
  {
    value: 20,
    color: "#878BB6",
  },
  {
    value: 40,
    color: "#4ACAB4",
  },
  {
    value: 10,
    color: "#FF8153",
  },
  {
    value: 30,
    color: "#FFEA88",
  },
];
```

Drawing a bar chart

```js
new Chart(income).Bar(barData);
```

```js
var barData = {
  labels: ["January", "February", "March", "April", "May", "June"],
  datasets: [
    {
      fillColor: "#48A497",
      strokeColor: "#48A4D1",
      data: [456, 479, 324, 569, 702, 600],
    },
    {
      fillColor: "rgba(73,188,170,0.4)",
      strokeColor: "rgba(72,174,209,0.4)",
      data: [364, 504, 605, 400, 345, 320],
    },
  ],
};
```

most of that are smiler

# canvas

At first sight a `<canvas>` looks like the `<img>` element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the `<canvas>` element has only two attributes, width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high. The element can be sized arbitrarily by CSS, but during rendering the image is scaled to fit its layout size: if the CSS sizing doesn't respect the ratio of the initial canvas, it will appear distorted.

- creates a fixed-size drawing surface that exposes one or more rendering contexts

### Drawing shapes with canvas

canvas grid or coordinate space Normally 1 unit in the grid corresponds to 1 pixel on the canvas. The origin of this grid is positioned in the top left corner at coordinate (0,0).

- only supports two primitive shapes: rectangles and paths (lists of points connected by lines). All other shapes must be created by combining one or more paths. Luckily, we have an assortment of path drawing functions which make it possible to compose very complex shapes.

- Drawing
  - First, you create the path.
  - Then you use drawing commands to draw into the path.
  - Once the path has been created, you can stroke or fill the path to render it.

### Colors

- fillStyle Sets the style used when filling shapes.
- strokeStyle Sets the style for shapes' outlines.

### Drawing text

`fillText(text, x, y [, maxWidth])`
`strokeText(text, x, y [, maxWidth])`
