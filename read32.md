# Summary
## The `<canvas>`

* At first sight a `<canvas>` looks like the` <img>` element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the` <canvas>` element has only two attributes, width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high. The element can be sized arbitrarily by CSS, but during rendering the image is scaled to fit its layout size: if the CSS sizing doesn't respect the ratio of the initial canvas, it will appear distorted.


* The `<canvas>` element differs from an` <img>` tag in that, like for `<video>` `<audio>,` or `<picture>` elements, it is easy to define some fallback content, to be displayed in older browsers not supporting it, like versions of Internet Explorer earlier than version 9 or textual browsers. You should always provide fallback content to be displayed by those browsers.

![image](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQrDkc6eVRlIbROYZ6KBQZcE4EeA6jI25D2bg&usqp=CAU.jpg)

## Drawing paths
 A path : is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color. A path, or even a subpath, can be closed. To make shapes using paths, we take some extra steps:

First, you create the path.
Then you use drawing commands to draw into the path.
Once the path has been created, you can stroke or fill the path to render it.
Here are the functions used to perform these steps:

### beginPath()
Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.
Path methods
Methods to set different paths for objects.
### closePath()
Adds a straight line to the path, going to the start of the current sub-path.
### stroke()
Draws the shape by stroking its outline.
### fill()
Draws a solid shape by filling the path's content area.
The first step to create a path is to call the beginPath(). Internally, paths are stored as a list of sub-paths (lines, arcs, etc) which together form a shape. Every time this method is called, the list is reset and we can start drawing new shapes.


## Applying styles and colors

### Colors
 * If we want to apply colors to a shape, there are two important properties we can use:` fillStyle` and strokeStyle.

## fillStyle = color
Sets the style used when filling shapes.
strokeStyle = color
Sets the style for shapes' outlines.
color is a string representing a CSS `<color>,` a gradient object, or a pattern object. We'll look at gradient and pattern objects later. By default, the stroke and fill color are set to black (CSS color value #000000).

![image](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRnN5GzFRK0rYwnbL87jdKer3FAeprfvjJdNg&usqp=CAU.jpg)


## Drawing text

### Drawing text
The canvas rendering context provides two methods to render text:

fillText(text, x, y [, maxWidth])
Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
strokeText(text, x, y [, maxWidth])
Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.
A fillText example
The text is filled using the current fillStyle.

![image](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQcdKIr5p2wt6_ONm8rA7879fjJIl0DjpJQRA&usqp=CAU.jpg)