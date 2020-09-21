# CANVAS 
At first sight a ```<canvas> ```looks like the ```<img>``` element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the ```<canvas>``` element has only two attributes, width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high.
- As a consequence of the way fallback is provided, unlike the ```<img>``` element, the <canvas> element requires the closing tag ```(</canvas>)```.
## The grid
Before we can start drawing, we need to talk about the canvas grid or coordinate space. Our HTML skeleton from the previous page had a canvas element 150 pixels wide and 150 pixels high. To the right, you see this canvas with the default grid overlayed. Normally 1 unit in the grid corresponds to 1 pixel on the canvas. The origin of this grid is positioned in the top left corner at coordinate (0,0).
## Drawing rectangles
```fillRect(x, y, width, height)```
Draws a filled rectangle.
```strokeRect(x, y, width, height)```
Draws a rectangular outline.
```clearRect(x, y, width, height)```
Clears the specified rectangular area, making it fully transparent.

## Drawing paths
```beginPath()```
Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.
```Path methods```
Methods to set different paths for objects.
```closePath()```
Adds a straight line to the path, going to the start of the current sub-path.
```stroke()```
Draws the shape by stroking its outline.
```fill()```
Draws a solid shape by filling the path's content area.
## Moving the pen
When the canvas is initialized or ```beginPath()``` is called, you typically will want to use the ```moveTo()``` function to place the starting point somewhere else. We could also use ```moveTo()``` to draw unconnected paths. Take a look at the smiley face below.
## Applying styles and colors:
- colors
```fillStyle = color```
Sets the style used when filling shapes.
```strokeStyle = color```
Sets the style for shapes' outlines.
- Transparency
```globalAlpha = transparencyValue```
Applies the specified transparency value to all future shapes drawn on the canvas. The value must be between 0.0 (fully transparent) to 1.0 (fully opaque). This value is 1.0 (fully opaque) by default.
- Drawing text
```fillText(text, x, y [, maxWidth])```
Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
```strokeText(text, x, y [, maxWidth])```
Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.
- Styling text
```font = value```, ```textAlign = value```, ```textBaseline = value```, ```direction = value```
