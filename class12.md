# Read: 12 - Docs for the HTML ```<canvas>``` Element & Chart.js

## EASILY CREATE STUNNING ANIMATED CHARTS WITH CHART.JS

![charts](https://www.qlik.com/blog/assets/uploads/images/posts/patrik-lundblad/pl-minichartspost-082820.png)

Charts are far better for displaying data visually than tables, A great way to get started with charts is with ***Chart.js***, a *JavaScript* plugin that uses HTML5’s canvas element to draw the graph onto the page.

1. Download Chart.js.(installation)
 You can get the latest version of Chart.js from [npm](https://www.npmjs.com/package/chart.js).
2. Copy the Chart.min.js into the directory you’ll be working in. 
3. HTML page
   + import the script:

    ```
    <script src='Chart.min.js'></script>
    ```
  
   + create a canvas element
 ```
 <canvas id="buyers" width="600" height="400"></canvas>
 ```
 4. write a script that will retrieve the context of the canvas
 ```
 <script>
    var buyers = document.getElementById('buyers').getContext('2d');
    new Chart(buyers).Line(buyerData);
</script>
 ```
5. create our data inside the same script tags
```
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
```
Notes:(Basic usage)

-the ```<canvas>``` element has only two attributes, **width and heigh**(These are both optional). 

-The **id** attribute isn't specific to the ```<canvas>``` element but is one of the global HTML attributes which can be applied to any HTML element (like class for instance).

-The ```<canvas>``` element *can be styled* just like any normal image (margin, border, background…).

-requires the closing tag ```</canvas>```.

### Drawing shapes with canvas
 Before we can start drawing, we need to talk about the canvas **grid** or **coordinate space**. 

 Normally 1 unit in the grid corresponds to 1 pixel on the canvas. The origin of this grid is positioned in the **top left** corner at coordinate (0,0). All elements are placed relative to this origin.


 * Drawing rectangles
 
 There are three functions that draw rectangles on the canvas:
   + fillRect(x, y, width, height) Draws a filled rectangle.
   + strokeRect(x, y, width, height) Draws a rectangular outline.
   + clearRect(x, y, width, height) Clears the specified rectangular area, making it fully transparent.

Note: 

x and y specify the **position** on the canvas (relative to the origin) of the top-left corner of the rectangle. width and height provide the rectangle's **size**.

### Applying styles and colors
#### **Colors**
two properties we can use: fillStyle and strokeStyle.
#### **Transparency**
globalAlpha property or by assigning a semi-transparent color to the stroke and/or fill style.
The value must be between 0.0 (fully transparent) to 1.0 (fully opaque). 
#### **Line styles**
* lineWidth = value
Sets the width of lines drawn in the future.

* lineCap = type
Sets the appearance of the ends of lines.

* lineJoin = type
Sets the appearance of the "corners" where lines meet.

* miterLimit = value
Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.

* getLineDash()

Returns the current line dash pattern array containing an even number of non-negative numbers.

* setLineDash(segments)
Sets the current line dash pattern.

* lineDashOffset = value
Specifies where to start a dash array on a line.

### Drawing text
![DT](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text/baselines.png)
The canvas rendering context provides two methods to render text:

* fillText(text, x, y [, maxWidth])

Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
* strokeText(text, x, y [, maxWidth])

Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.