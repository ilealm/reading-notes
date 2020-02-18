# Read 12 Assorted bits of documentation

### February 17th, 2020


### _Charts_
* The canvas element creates a fixed-size drawing surface that exposes one or more _**rendering contexts**_.
* We can create a chart on a page using the  \<canvas\> element.
  * _Sintax_
  \<canvas id="myChart" width="400" height="400"\>\</canvas\>
* Canvas element have these attributes: id, width and hight. With and hight are optionl, and when they are not indicatted take the value of 300px and 150px respectively.
* The canvas element can be styled as any image .
* If the browser does not suppot canvas element, we can use a fallback element to display insted.
* Canvas element requiere a closing tag, if is not present, the rest of the document will be considered as fallback.
* The \<canvas\> element has a method called getContext(), used to obtain the rendering context and its drawing functions.
* Canvas is a space where we can create drawings.
* To possition elements on the canvas, we need to work with _**the grid**_, which is a coordinate space.
* Normally 1 unit in the grid corresponds to 1 pixel on the canvas. 
* The origin of this grid is positioned in the top left corner at coordinate (0,0)

### _Recyangle Figure_
_**fillRect(x, y, width, height)**_
  Draws a filled rectangle.

_**strokeRect(x, y, width, height)**_
  Draws a rectangular outline.

_**clearRect(x, y, width, height)**_
  Clears the specified rectangular area, making it fully transparent.

### _Paths_
* A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color.

#### Steps to create a path:
  1. Creeate the path.
  1. Use drawing commands to draw into the path.
  1. Once the path has been created, you can stroke or fill the path to render it.

  _*Functions to accomplish these steps*_
  _**cbeginPath()**_
    Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.
  _**Path methods**_
  Methods to set different paths for objects.

  _**cclosePath()**_
  Adds a straight line to the path, going to the start of the current sub-path.

  _**stroke()**_
  Draws the shape by stroking its outline.

  _**fill()**_
  Draws a solid shape by filling the path's content area.

  #### _*Example*_
  ctx.beginPath();
  ctx.moveTo(75, 50);
  ctx.lineTo(100, 75);
  ctx.lineTo(100, 25);
  ctx.fill();

### _Arcs_
* To draw arcs or circles, we use the arc() or arcTo() methods.
 * _Sintax_
  arc(x, y, radius, startAngle, endAngle, anticlockwise)

### _Bezier and quadratic curves_
* These are generally used to draw complex organic shapes, and are available in both cubic and quadratic varieties.

_**quadraticCurveTo(cp1x, cp1y, x, y)*_
Draws a quadratic Bézier curve from the current pen position to the end point specified by x and y, using the control point specified by cp1x and cp1y.

_**bezierCurveTo(cp1x, cp1y, cp2x, cp2y, x, y)*_
Draws a cubic Bézier curve from the current pen position to the end point specified by x and y, using the control points specified by (cp1x, cp1y) and (cp2x, cp2y).

### _Colors_

_**fillStyle = color**_
Sets the style used when filling shapes.

_**strokeStyle = color**_
Sets the style for shapes' outlines.

### _Line Styles_

_**lineWidth = value**_
Sets the width of lines drawn in the future.

_**lineCap = type**_
Sets the appearance of the ends of lines.

_**lineJoin = type**_
Sets the appearance of the "corners" where lines meet.

_**miterLimit = value**_
Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.

_**getLineDash()**_
Returns the current line dash pattern array containing an even number of non-negative numbers.

_**setLineDash(segments)**_
Sets the current line dash pattern.

_**lineDashOffset = value**_
Specifies where to start a dash array on a line.

### _Gradients_
* We can fill and stroke shapes using linear and radial gradients.

 * _Sintax_
  createLinearGradient(x1, y1, x2, y2)

### _Patterns_
  * _Sintax_
  createPattern(image, type)

  * image is a CanvasImageSource.
  * The type specifies how to use the image in order to create the pattern, and must be one of the following string values:

  _**repeat**_
  Tiles the image in both vertical and horizontal directions.

  _**repeat-x**_
  Tiles the image horizontally but not vertically.

  _**repeat-y**_
  Tiles the image vertically but not horizontally.

  _**no-repeat**_
  Doesn't tile the image. It's used only once.

### _Shadows_
* Using shadows involves just four properties:
  
   _**shadowOffsetX = float**_
  Indicates the horizontal distance the shadow should extend from the object. This value isn't affected by the transformation matrix. The default is 0.
  
   _**shadowOffsetY = float**_
  Indicates the vertical distance the shadow should extend from the object. This value isn't affected by the transformation matrix. The default is 0.
  
   _**shadowBlur = float**_
  Indicates the size of the blurring effect; this value doesn't correspond to a number of pixels and is not affected by the current transformation matrix. The default value is 0.
  
   _**shadowColor = color**_
  A standard CSS color value indicating the color of the shadow effect; by default, it is fully-transparent black.

### _Drawing text_
  * The canvas rendering context provides two methods to render text:

  _**fillText(text, x, y [, maxWidth])**_
  Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
  
  _**strokeText(text, x, y [, maxWidth])**_
  Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

### _Styling text_
  * There are some more properties which let you adjust the way the text gets displayed on the canvas:
  
  _**font = value**_
  The current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.
  
  _**textAlign = value**_
  Text alignment setting. Possible values: start, end, left, right or center. The default value is start.
  
  _**textBaseline = value**_
  Baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.
  
  _**direction = value**_
  Directionality. Possible values: ltr, rtl, inherit. The default value is inherit.