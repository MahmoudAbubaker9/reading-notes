# Chart.js API.

Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.

A great way to get started with charts is with Chart.js, a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page. It’s a well documented plugin that makes using all kinds of bar charts, line charts, pie charts and more, incredibly easy.

**Basic usage of canvas**

At first sight a canvas looks like the img element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the canvas element has only two attributes, width and height. These are both optional and can also be set using DOM properties.

Note: If your renderings seem distorted, try specifying your width and height attributes explicitly in the canvas attributes, and not using CSS.

**canvas grid**

![img](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes/canvas_default_grid.png)

Normally 1 unit in the grid corresponds to 1 pixel on the canvas. The origin of this grid is positioned in the top left corner at coordinate (0,0). All elements are placed relative to this origin. So the position of the top left corner of the blue square becomes x pixels from the left and y pixels from the top, at coordinate (x,y). Later in this tutorial we'll see how we can translate the origin to a different position, rotate the grid and even scale it, but for now we'll stick to the default.

**Drawing rectangles**

![img](https://mdn.mozillademos.org/files/245/Canvas_rect.png)

Unlike SVG, anvas only supports two primitive shapes: rectangles and paths (lists of points connected by lines). All other shapes must be created by combining one or more paths. Luckily, we have an assortment of path drawing functions which make it possible to compose very complex shapes.

First let's look at the rectangle. There are three functions that draw rectangles on the canvas:

fillRect(x, y, width, height)
Draws a filled rectangle.
strokeRect(x, y, width, height)
Draws a rectangular outline.
clearRect(x, y, width, height)
Clears the specified rectangular area, making it fully transparent.
Each of these three functions takes the same parameters. x and y specify the position on the canvas (relative to the origin) of the top-left corner of the rectangle. width and height provide the rectangle's size.

Drawing paths
Now let's look at paths. A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color. A path, or even a subpath, can be closed. To make shapes using paths, we take some extra steps:

First, you create the path.
Then you use drawing commands to draw into the path.
Once the path has been created, you can stroke or fill the path to render it.
Here are the functions used to perform these steps:

beginPath()

Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.

**Path methods**

Methods to set different paths for objects.

closePath()

Adds a straight line to the path, going to the start of the current sub-path.

stroke()

Draws the shape by stroking its outline.

fill()

Draws a solid shape by filling the path's content area.

The first step to create a path is to call the beginPath(). Internally, paths are stored as a list of sub-paths (lines, arcs, etc) which together form a shape. Every time this method is called, the list is reset and we can start drawing new shapes.

The second step is calling the methods that actually specify the paths to be drawn. We'll see these shortly.

The third, and an optional step, is to call closePath(). This method tries to close the shape by drawing a straight line from the current point to the start. If the shape has already been closed or there's only one point in the list, this function does nothing.

**Applying styles and colors**

Up until now we have only seen methods of the drawing context. If we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle.

fillStyle = color

Sets the style used when filling shapes.

strokeStyle = color

Sets the style for shapes' outlines.

* color is a string representing a CSS color, a gradient object, or a pattern object. We'll look at gradient and pattern objects later. By default, the stroke and fill color are set to black (CSS color value #000000).

**Line styles**

There are several properties which allow us to style lines.

lineWidth = value

Sets the width of lines drawn in the future.

lineCap = type

Sets the appearance of the ends of lines.

lineJoin = type

Sets the appearance of the "corners" where lines meet.

miterLimit = value

Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.

getLineDash()

Returns the current line dash pattern array containing an even number of non-negative numbers.

setLineDash(segments)

Sets the current line dash pattern.

lineDashOffset = value

Specifies where to start a dash array on a line.


**Gradients**

Just like any normal drawing program, we can fill and stroke shapes using linear, radial and conic gradients. We create a CanvasGradient object by using one of the following methods. We can then assign this object to the fillStyle or strokeStyle properties.

createLinearGradient(x1, y1, x2, y2)

Creates a linear gradient object with a starting point of (x1, y1) and an end point of (x2, y2).

createRadialGradient(x1, y1, r1, x2, y2, r2)

Creates a radial gradient. The parameters represent two circles, one with its center at (x1, y1) and a radius of r1, and the other with its center at (x2, y2) with a radius of r2.

createConicGradient(angle, x, y)

Creates a conic gradient object with a starting angle of angle in radians, at the position (x, y).

**Shadows**

Using shadows involves just four properties:

shadowOffsetX = float

Indicates the horizontal distance the shadow should extend from the object. This value isn't affected by the transformation matrix. The default is 0.

shadowOffsetY = float

Indicates the vertical distance the shadow should extend from the object. This value isn't affected by the transformation matrix. The default is 0.

shadowBlur = float

Indicates the size of the blurring effect; this value doesn't correspond to a number of pixels and is not affected by the current transformation matrix. The default value is 0.

shadowColor = color

A standard CSS color value indicating the color of the shadow effect; by default, it is fully-transparent black.

**Drawing text**

The canvas rendering context provides two methods to render text:

fillText(text, x, y [, maxWidth])

Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.

strokeText(text, x, y [, maxWidth])

Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

**Styling text**

In the examples above we are already making use of the font property to make the text a bit larger than the default size. There are some more properties which let you adjust the way the text gets displayed on the canvas:

font = value

The current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.

textAlign = value

Text alignment setting. Possible values: start, end, left, right or center. The default value is start.

textBaseline = value

Baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.

direction = value

Directionality. Possible values: ltr, rtl, inherit. The default value is inherit.

**Advanced text measurements**

In the case you need to obtain more details about the text, the following method allows you to measure it.

measureText()

Returns a TextMetrics object containing the width, in pixels, that the specified text will be when drawn in the current text style.