# Canvas

## Basic usage
### The basic structure of a canvas:

```
<canvas id="idName" width="150" height="150"></canvas>
```

The canvas element has only two attributes, **width** and **height**, the **id** attribute is used for styling or set values for it's attributes using the **DOM properties**.

### Fallback contant:
The **canvas** element isn't supported in some older browsers, so you can add some **fallback contant** to be displayed in them. **ex**:

```
<canvas id="clock" width="150" height="150">
  <img src="images/clock.png" width="150" height="150" alt=""/>
</canvas>
```

If the browser suppots the **canvas** element it will ignore the contant and display the **canvas** it self, otherwise the contant of the **canvas** element will be displayed and the **canvas** will be ignored.

**Note**: the closing tag is required for the **canvas** element.

**Note**: the support of the **canvas** for the browser can be tested by using a **js** code that checks for the `getcontext()` method.

## Drawing shapes with canvas
### The grid:
The **origin point** of the grid is the **top-left corner** at *(0, 0)* (x pixels from the left, y pixels from the top), each unit in the grid usually corresponds to a pixel on the **canvas**.

The canvas element supports only two primative shapes, these are **rectangles** and **paths**, and there are funcations that help us to draw them:

- **For Rectangles**:
    - **fillRect(x, y, width, height)**: draws a filled rectangle.
    - **strokeRect(x, y, width, height)**: draws a rectangular outline.
    - **clearRect(x, y, width, height)**: clears the specifiedrectangular area, making it fully transparent.

    **Note**: these functions are drawn immediately.

- **For Paths**: 
    - **BeginPath()**: creates a new path that future drawing commands are directed into. 
    - **closePath()**: adds a straight line to the path, going to the start of the current sub-path.
    - **stroke()**: draws the shape by stroking its outline.
    - **fill()**: draws a solid shape by filling the path's content area.
    **Notes**: 
        paths are lists of points, connected by segments of lines that can be of different shapes.

        Inorder to make a shape using paths you need to:
        1. Create a path.
        2. Using **drawing commands** to draw into the created path.
        3. Stroke or fill the path in order to render it.

#### Moving the pen: `moveTo(x, y)` moves the pen to the coordinates specified by x and y.

#### Lines: `lineTo(x, y)` draws a line from the current drawing position to the position specified by x and y.

#### Arcs: 
 - **arc(x, y, radius, startAngle, endAngle, counterclockwise)**: draws an arc which is centered at (x, y) position with radius r starting at startAngle and ending at endAngle going in the given direction indicated by counterclockwise
 - **arcTo(x1, y1, x2, y2, radius)**: draws an arc with the given control points and radius, connected to the previous point by a straight line.

## Applying styles and colors
### Colors:
**To apply colors**:
- **fillStyle = color**: sets the style used when filling shapes.
- **strokeStyle = color**: sets the style for shapes' outlines.

### Transparency:
**To set transparency**: `globalAlpha = transparencyValue`.

### Line Styles:
**To apply line styles**:
- **lineWidth = value**: sets the width of lines drawn in the future.
- **lineCap = type**: sets the appearance of the ends of lines.
- **lineJoin = type**: sets the appearance of the "corners" where lines meet.
- **miterLimit = value**: limits the miter when two lines join at a sharp angle.
- **getLineDash()**: returns the current line dash pattern array containing an even number of non-negative numbers.
- **setLineDash(segments)**: sets the current line dash pattern.
- **lineDashOffset = value**: specifies where to start a dash array on a line.

### Gradients:
**To create a gradient**:
- **createLinearGradient(x1, y1, x2, y2)**: creates a linear gradient object with a starting point of (x1, y1) and an end point of (x2, y2).
- **createRadialGradient(x1, y1, r1, x2, y2, r2)**: creates a radial gradient. The parameters represent two circles, one with its center at (x1, y1) and a radius of r1, and the other with its center at (x2, y2) with a radius of r2.
- **createConicGradient(angle, x, y)**: creates a conic gradient object with a starting angle of angle in radians, at the position (x, y).

### Patterns:
**To create a pattern**:

**createPattern(image, type)**: creates and returns a new canvas pattern object.

**Pattern types**:
- *repeat*: tiles the image in both vertical and horizontal directions.
- *repeat-x*: tiles the image horizontally but not vertically.
- *repeat-y*: tiles the image vertically but not horizontally.
- *no-repeat*: doesn't tile the image. It's used only once.

### Shadows
**Shadow properties**:
- **shadowOffsetX = float**: indicates the horizontal distance the shadow should extend from the object. This value isn't affected by the transformation matrix. The default is 0.
- **shadowOffsetY = float**: indicates the vertical distance the shadow should extend from the object. This value isn't affected by the transformation matrix. The default is 0.
- **shadowBlur = float**: indicates the size of the blurring effect; this value doesn't correspond to a number of pixels and is not affected by the current transformation matrix. The default value is 0.
- **shadowColor = color**: standard CSS color value indicating the color of the shadow effect; by default, it is fully-transparent black.

## Drawing text

**To draw text**:
- **fillText(text, x, y [, maxWidth])**: fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
- **strokeText(text, x, y [, maxWidth])**: strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

**To style text**: 
- **font = value**
- **textAlign = value**
- **textBaseline = value**: saseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.
- **direction = value**
