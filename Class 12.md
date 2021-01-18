> # Class 12 *Jan 18 2021:*

> ## Topics

  1. Chart.js [Referance](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/) [Documention](https://www.chartjs.org/docs/latest/)
  
  2. Canvas
  


---

> ## 1. Chart.js

![Chart.js](https://i.morioh.com/2020/04/30/8e58b48c35cf.jpg)

----


**Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.**

#### Setting up

  1. Download Chart.js: you can find the Chart.js library [here](https://github.com/chartjs/Chart.js)

  2. You can also include it from the cdn by using the script tag `<script src="https://cdn.jsdelivr.net/npm/chart.js@2.8.0"></script>`

----

#### Drawing a line chart  

* **To draw a line chart, the first thing we need to do is create a canvas element in our HTML in which Chart.js can draw our chart. So add this to the body of our HTML page:**

  1. `<canvas id="buyers" width="600" height="400"></canvas>`

  2. `<script> var buyers = document.getElementById('buyers').getContext('2d');     new Chart(buyers).Line(buyerData);</script>`

  3. Inside the same script tags we need to create our data, in this instance it’s an object that contains labels for the base of our chart and datasets to describe the values on the chart.

        var buyerData = {
        labels : ["January","February","March","April","May","June"],
        datasets : [
          {
            fillColor : "rgba(172,194,132,0.4)",
            strokeColor : "#ACC26D",
            pointColor : "#fff",
            pointStrokeColor : "#9DB86D",
            data : [203,156,99,251,305,247]
          }
        ]
      }

----

#### Drawing a pie chart

  1. Our line chart is complete, so let’s move on to our pie chart. First, we need the canvas element:

        <canvas id="countries" width="600" height="400"></canvas>

  2. Next, we need to get the context and to instantiate the chart:

        var countries= document.getElementById("countries").getContext("2d");
        new Chart(countries).Pie(pieData, pieOptions);

  3. Next we need to create the data. This data is a little different to the line chart because the pie chart is simpler, we just need to supply a value and a color for each section:

        var pieData = [
        {
          value: 20,
          color:"#878BB6"
        },
        {
          value : 40,
          color : "#4ACAB4"
        },
        {
          value : 10,
          color : "#FF8153"
        },
        {
          value : 30,
          color : "#FFEA88"
        }
      ];

      var pieOptions = {
      segmentShowStroke : false,
      animateScale : true
    }

----

#### Drawing a bar chart:

  1. we add the canvas element:

        `<canvas id="income" width="600" height="400"></canvas>`

  2.  retrieve the element and create the graph:

        var income = document.getElementById("income").getContext("2d");
        new Chart(income).Bar(barData);

  3.  add in the bar chart’s data:

        var barData = {
        labels : ["January","February","March","April","May","June"],
        datasets : [
          {
            fillColor : "#48A497",
            strokeColor : "#48A4D1",
            data : [456,479,324,569,702,600]
          },
          {
            fillColor : "rgba(73,188,170,0.4)",
            strokeColor : "rgba(72,174,209,0.4)",
            data : [364,504,605,400,345,320]
          }

        ]
      }

----

#### Try to Copy the Example Below:

      <!DOCTYPE html>
      <html lang="en">
          <head>
              <meta charset="utf-8" />
              <title>Chart.js demo</title>
              <!-- import plugin script -->
              <script src='Chart.min.js'></script>
          </head>
          <body>
              <!-- line chart canvas element -->
              <canvas id="buyers" width="600" height="400"></canvas>
              <!-- pie chart canvas element -->
              <canvas id="countries" width="600" height="400"></canvas>
              <!-- bar chart canvas element -->
              <canvas id="income" width="600" height="400"></canvas>
              <script>
                  // line chart data
                  var buyerData = {
                      labels : ["January","February","March","April","May","June"],
                      datasets : [
                      {
                          fillColor : "rgba(172,194,132,0.4)",
                          strokeColor : "#ACC26D",
                          pointColor : "#fff",
                          pointStrokeColor : "#9DB86D",
                          data : [203,156,99,251,305,247]
                      }
                  ]
                  }
                  // get line chart canvas
                  var buyers = document.getElementById('buyers').getContext('2d');
                  // draw line chart
                  new Chart(buyers).Line(buyerData);
                  // pie chart data
                  var pieData = [
                      {
                          value: 20,
                          color:"#878BB6"
                      },
                      {
                          value : 40,
                          color : "#4ACAB4"
                      },
                      {
                          value : 10,
                          color : "#FF8153"
                      },
                      {
                          value : 30,
                          color : "#FFEA88"
                      }
                  ];
                  // pie chart options
                  var pieOptions = {
                      segmentShowStroke : false,
                      animateScale : true
                  }
                  // get pie chart canvas
                  var countries= document.getElementById("countries").getContext("2d");
                  // draw pie chart
                  new Chart(countries).Pie(pieData, pieOptions);
                  // bar chart data
                  var barData = {
                      labels : ["January","February","March","April","May","June"],
                      datasets : [
                          {
                              fillColor : "#48A497",
                              strokeColor : "#48A4D1",
                              data : [456,479,324,569,702,600]
                          },
                          {
                              fillColor : "rgba(73,188,170,0.4)",
                              strokeColor : "rgba(72,174,209,0.4)",
                              data : [364,504,605,400,345,320]
                          }
                      ]
                  }
                  // get bar chart canvas
                  var income = document.getElementById("income").getContext("2d");
                  // draw bar chart
                  new Chart(income).Bar(barData);
              </script>
          </body>
      </html>

---

> ## 2. Canvas


 * **The HTML <canvas> element is used to draw graphics on a web page. The graphic to the left is created with <canvas>. It shows four elements: a red rectangle, a gradient rectangle, a multicolor rectangle, and a multicolor text.**   

----

#### Basic Canavs:

 **Canvas Exampe:** `<canvas id="tutorial" width="150" height="150"></canvas>`

 **`<canvas>` looks like the `<img>` element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the `<canvas>` element has only two attributes, width and height. These are both optional and can also be set using DOM properties**


**Example:**

      <canvas id="stockGraph" width="150" height="150">
        current stock price: $3.15 + 0.15
      </canvas>

      <canvas id="clock" width="150" height="150">
        <img src="images/clock.png" width="150" height="150" alt=""/>
      </canvas>

----

#### Drawing shapes

* **The grid**

we need to talk about the canvas grid or coordinate space. Our HTML skeleton from the previous page had a canvas element 150 pixels wide and 150 pixels high. To the right, you see this canvas with the default grid overlayed. Normally 1 unit in the grid corresponds to 1 pixel on the canvas. The origin of this grid is positioned in the top left corner at coordinate (0,0). All elements are placed relative to this origin. So the position of the top left corner of the blue square becomes x pixels from the left and y pixels from the top, at coordinate (x,y). Later in this tutorial we'll see how we can translate the origin to a different position, rotate the grid and even scale it, but for now we'll stick to the default.


![The grid](https://miro.medium.com/max/1668/1*o1I8eC5nQdyuAABzJYg3iQ.png)

----

* **Drawing rectangles**

**There are three functions that draw rectangles on the canvas:**

  1. `fillRect(x, y, width, height)`: Draws a filled rectangle.

  2. `strokeRect(x, y, width, height)`: Draws a rectangular outline.

  3. `clearRect(x, y, width, height)`: Clears the specified rectangular area, making it fully transparent.


**Example:** 

      function draw() {
      var canvas = document.getElementById('canvas');
      if (canvas.getContext) {
        var ctx = canvas.getContext('2d');

        ctx.fillRect(25, 25, 100, 100);
        ctx.clearRect(45, 45, 60, 60);
        ctx.strokeRect(50, 50, 50, 50);
      }
    }



![Canvas Rectangle](https://i.ytimg.com/vi/AD0u6LweP1g/mqdefault.jpg)


----

* **Drawing paths and Triangle:** A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color. A path, or even a subpath, can be closed. To make shapes using paths, we take some extra steps:

  1. First, you create the path.
  
  2. Then you use drawing commands to draw into the path.

  3. Once the path has been created, you can stroke or fill the path to render it.

**The functions used to perform these steps:**

  1. `beginPath()`: Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.

  2. Path methods: Methods to set different paths for objects.

  3. `closePath()`: Adds a straight line to the path, going to the start of the current sub-path.

  4. `stroke()`: Draws the shape by stroking its outline.

  5. `fill()`: Draws a solid shape by filling the path's content area.


  ![beginPath](https://i.stack.imgur.com/5mlqv.png)

**Example:**

      function draw() {
      var canvas = document.getElementById('canvas');
      if (canvas.getContext) {
        var ctx = canvas.getContext('2d');

        ctx.beginPath();
        ctx.moveTo(75, 50);
        ctx.lineTo(100, 75);
        ctx.lineTo(100, 25);
        ctx.fill();
      }
    }

---

* **Moving the pen**: One very useful function, which doesn't actually draw anything but becomes part of the path list described above, is the `moveTo()` function. You can probably best think of this as lifting a pen or pencil from one spot on a piece of paper and placing it on the next.


  * `moveTo(x, y)`: Moves the pen to the coordinates specified by x and y. 

![Moving the pen](https://www.programmingbasics.org/en/downloads/html5canvas/img/htmlcanvas%20-%20023.png)

**Example:**

      function draw() {
      var canvas = document.getElementById('canvas');
      if (canvas.getContext) {
        var ctx = canvas.getContext('2d');

        ctx.beginPath();
        ctx.arc(75, 75, 50, 0, Math.PI * 2, true); // Outer circle
        ctx.moveTo(110, 75);
        ctx.arc(75, 75, 35, 0, Math.PI, false);  // Mouth (clockwise)
        ctx.moveTo(65, 65);
        ctx.arc(60, 65, 5, 0, Math.PI * 2, true);  // Left eye
        ctx.moveTo(95, 65);
        ctx.arc(90, 65, 5, 0, Math.PI * 2, true);  // Right eye
        ctx.stroke();
      }
    }

----

* **Lines**:For drawing straight lines, use the `lineTo()` method.


**Example:**

      function draw() {
      var canvas = document.getElementById('canvas');
      if (canvas.getContext) {
        var ctx = canvas.getContext('2d');

        // Filled triangle
        ctx.beginPath();
        ctx.moveTo(25, 25);
        ctx.lineTo(105, 25);
        ctx.lineTo(25, 105);
        ctx.fill();

        // Stroked triangle
        ctx.beginPath();
        ctx.moveTo(125, 125);
        ctx.lineTo(125, 45);
        ctx.lineTo(45, 125);
        ctx.closePath();
        ctx.stroke();
      }
    }


----

* **Arcs** To draw arcs or circles, we use the `arc()` or `arcTo()` methods.

  1. `arc(x, y, radius, startAngle, endAngle, anticlockwise)`:Draws an arc which is centered at (x, y) position with radius r starting at startAngle and ending at endAngle going in the given direction indicated by anticlockwise (defaulting to clockwise).

  2. `arcTo(x1, y1, x2, y2, radius)`: Draws an arc with the given control points and radius, connected to the previous point by a straight line.

**Example:**

        function draw() {
        var canvas = document.getElementById('canvas');
        if (canvas.getContext) {
          var ctx = canvas.getContext('2d');

          for (var i = 0; i < 4; i++) {
            for (var j = 0; j < 3; j++) {
              ctx.beginPath();
              var x = 25 + j * 50; // x coordinate
              var y = 25 + i * 50; // y coordinate
              var radius = 20; // Arc radius
              var startAngle = 0; // Starting point on circle
              var endAngle = Math.PI + (Math.PI * j) / 2; // End point on circle
              var anticlockwise = i % 2 !== 0; // clockwise or anticlockwise

              ctx.arc(x, y, radius, startAngle, endAngle, anticlockwise);

              if (i > 1) {
                ctx.fill();
              } else {
                ctx.stroke();
              }
            }
          }
        }
      }


----

* **Bezier and quadratic curves**

  1. `quadraticCurveTo(cp1x, cp1y, x, y)`: Draws a quadratic Bézier curve from the current pen position to the end point specified by x and y, using the control point specified by cp1x and cp1y.

  2. `bezierCurveTo(cp1x, cp1y, cp2x, cp2y, x, y)`:  Draws a cubic Bézier curve from the current pen position to the end point specified by x and y, using the control points specified by (cp1x, cp1y) and (cp2x, cp2y).

![Bezier and quadratic curves](https://mdn.mozillademos.org/files/223/Canvas_curves.png)

**Example:**

      function draw() {
      var canvas = document.getElementById('canvas');
      if (canvas.getContext) {
        var ctx = canvas.getContext('2d');

        // Quadratric curves example
        ctx.beginPath();
        ctx.moveTo(75, 25);
        ctx.quadraticCurveTo(25, 25, 25, 62.5);
        ctx.quadraticCurveTo(25, 100, 50, 100);
        ctx.quadraticCurveTo(50, 120, 30, 125);
        ctx.quadraticCurveTo(60, 120, 65, 100);
        ctx.quadraticCurveTo(125, 100, 125, 62.5);
        ctx.quadraticCurveTo(125, 25, 75, 25);
        ctx.stroke();
      }
    }


----

#### Applying styles and colors:

* **To Applye Styles an color use these methods**

  1. color fill

    1. `fillStyle = color`: Sets the style used when filling shapes.

    2. `strokeStyle = color`: Sets the style for shapes' outlines.

  2. Transparency

    1. `globalAlpha = transparencyValue`: Applies the specified transparency value to all future shapes drawn on the canvas. The value must be between 0.0 (fully transparent) to 1.0 (fully opaque). This value is 1.0 (fully opaque) by default.

  3. Line styles:
    
    1. `lineWidth = value`: Sets the width of lines drawn in the future.

    2. `lineCap = type`: Sets the appearance of the ends of lines.

    3. `lineJoin = type`: Sets the appearance of the "corners" where lines meet.

    4. `miterLimit = value`: Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.

    5. `getLineDash()`: Returns the current line dash pattern array containing an even number of non-negative numbers.

    6. `setLineDash(segments)`: Sets the current line dash pattern.

    7. `lineDashOffset = value`: Specifies where to start a dash array on a line.

  4. Gradients: 

    1. `createLinearGradient(x1, y1, x2, y2)`: Creates a linear gradient object with a starting point of (x1, y1) and an end point of (x2, y2).

    2. `createRadialGradient(x1, y1, r1, x2, y2, r2)`: Creates a radial gradient. The parameters represent two circles, one with its center at (x1, y1) and a radius of r1, and the other with its center at (x2, y2) with a radius of r2.

    3. `gradient.addColorStop(position, color)`: Creates a new color stop on the gradient object. The position is a number between 0.0 and 1.0 and defines the relative position of the color in the gradient, and the color argument must be a string representing a CSS `<color>`, indicating the color the gradient should reach at that offset into the transition.

  5. Patterns:

    1. `createPattern(image, type)`: Creates and returns a new canvas pattern object. image is a CanvasImageSource (that is, an HTMLImageElement, another canvas, a `<video>` element, or the like. type is a string indicating how to use the image.

    2. `repeat`: Tiles the image in both vertical and horizontal directions.

    3. `repeat-x`: Tiles the image horizontally but not vertically.

    4. `repeat-y`: Tiles the image vertically but not horizontally.

    5. `no-repeat`: Doesn't tile the image. It's used only once.


----

#### Drawing text:

* **The canvas rendering context provides two methods to render text:**

  1. `fillText(text, x, y [, maxWidth])`: Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.

  2. `strokeText(text, x, y [, maxWidth])`:Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

----

* **Styling text:** you can adjust the text gets displayed on the canvas:

  1. `font = value`: The current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.

  2. `textAlign = value`: Text alignment setting. Possible values: start, end, left, right or center. The default value  is start.

  3. `textBaseline = value`: Baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.

  4. `direction = value`: Directionality. Possible values: ltr, rtl, inherit. The default value is inherit.



----

* **Advanced text measurements:** In the case you need to obtain more details about the text, the following method allows you to measure it.

  1. `measureText()`: Returns a TextMetrics object containing the width, in pixels, that the specified text will be when drawn in the current text style.

---

![cheat sheet](https://mk0wittysparksm75pi6.kinstacdn.com/wp-content/uploads/2017/07/HTML-Canvas-Cheatsheet.png)

---
Github Live: [view](https://anassawalha95.github.io/reading-notes-2/Class%2012)

Github Repo: [view](https://github.com/anassawalha95/reading-notes-2/blob/main/Class%2012.md)
