Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.

# Drawing a line chart
To draw a line chart, the first thing we need to do is create a canvas element in our HTML in which Chart.js can draw our chart. So add this to the body of our HTML page:
` <canvas id="buyers" width="600" height="400"></canvas> `
Next, we need to write a script that will retrieve the context of the canvas, so add this to the foot of your body element:
```
<script>
    var buyers = document.getElementById('buyers').getContext('2d');
    new Chart(buyers).Line(buyerData);
</script>

```
Inside the same script tags we need to create our data, in this instance it’s an object that contains labels for the base of our chart and datasets to describe the values on the chart. Add this immediately above the line that begins ‘var buyers=’:
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
# Drawing a pie chart
Our line chart is complete, so let’s move on to our pie chart. First, we need the canvas element:
`<canvas id="countries" width="600" height="400"></canvas>`
Next, we need to get the context and to instantiate the chart:
```
var countries= document.getElementById("countries").getContext("2d");
new Chart(countries).Pie(pieData, pieOptions);
```
You’ll notice that this time, we are going to supply some options to the chart.

```
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
```
Now, immediately after the pieData we’ll add our options:
```
var pieOptions = {
	segmentShowStroke : false,
	animateScale : true
}
```
# The `<canvas>` element
At first sight a `<canvas>` looks like the `<img>` element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the `<canvas>` element has only two attributes, width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high. The element can be sized arbitrarily by CSS, but during rendering the image is scaled to fit its layout size: if the CSS sizing doesn't respect the ratio of the initial canvas, it will appear distorted.

# Fallback content
The `<canvas>` element differs from an `<img>` tag in that, like for `<video>`, `<audio>`, or `<picture>` elements, it is easy to define some fallback content, to be displayed in older browsers not supporting it, like versions of Internet Explorer earlier than version 9 or textual browsers. You should always provide fallback content to be displayed by those browsers.

# Required `</canvas>` tag
As a consequence of the way fallback is provided, unlike the `<img>` element, the `<canvas>` element requires the closing tag (`</canvas>`). If this tag is not present, the rest of the document would be considered the fallback content and wouldn't be displayed.

# The rendering context
The `<canvas>` element creates a fixed-size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown. In this tutorial, we focus on the 2D rendering context. Other contexts may provide different types of rendering.
`getContext()` takes one parameter, the type of context. For 2D graphics, such as those covered by this tutorial, you specify "2d" to get a `CanvasRenderingContext2D`.

# Checking for support
The fallback content is displayed in browsers which do not support `<canvas>`. Scripts can also check for support programmatically by testing for the presence of the `getContext()` method.

# The grid
## Drawing rectangles
Unlike SVG, `<canvas>` only supports two primitive shapes: rectangles and paths (lists of points connected by lines). All other shapes must be created by combining one or more paths. Luckily, we have an assortment of path drawing functions which make it possible to compose very complex shapes.

First let's look at the rectangle. There are three functions that draw rectangles on the canvas:

`fillRect(x, y, width, height)`
Draws a filled rectangle.
`strokeRect(x, y, width, height)`
Draws a rectangular outline.
`clearRect(x, y, width, height)`
Clears the specified rectangular area, making it fully transparent.

`beginPath()`
Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.
`Path methods`
Methods to set different paths for objects.
`closePath()`
Adds a straight line to the path, going to the start of the current sub-path.
`stroke()`
Draws the shape by stroking its outline.
`fill()`
Draws a solid shape by filling the path's content area.
# Moving the pen
One very useful function, which doesn't actually draw anything but becomes part of the path list described above, is the `moveTo()` function. You can probably best think of this as lifting a pen or pencil from one spot on a piece of paper and placing it on the next.
`moveTo(x, y)`
Moves the pen to the coordinates specified by x and y.
`lineTo(x, y)`
Draws a line from the current drawing position to the position specified by x and y.
`arc(x, y, radius, startAngle, endAngle, anticlockwise)`
`arcTo(x1, y1, x2, y2, radius)`
`Path2D()`
The `Path2D()` constructor returns a newly instantiated `Path2D` object, optionally with another path as an argument (creates a copy), or optionally with a string consisting of SVG path data.
`fillStyle = color`
Sets the style used when filling shapes.
`strokeStyle = color`
Sets the style for shapes' outlines.
color is a string representing a CSS`<color>`, a gradient object, or a pattern object. We'll look at gradient and pattern objects later. By default, the stroke and fill color are set to black (CSS color value #000000).

# Drawing text
The canvas rendering context provides two methods to render text:

`fillText(text, x, y [, maxWidth])`
Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
`strokeText(text, x, y [, maxWidth])`
Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

`font = value`
The current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.
`textAlign = value`
Text alignment setting. Possible values: start, end, left, right or center. The default value is start.
`textBaseline = value`
Baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.
`direction = value`
Directionality. Possible values: ltr, rtl, inherit. The default value is inherit.