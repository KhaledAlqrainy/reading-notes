# Charts.js

> Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.

# Canvas elements:

> the "canvas" element has only two attributes, width and height. These are both optional and can also be set using DOM properties. 

* if there is now width or hieght included tha standard values of it will be **300 pixels wide** and **150 pixels high**.

* The "canvas" element creates a fixed-size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown.

### Applying styles and colors:

* **Color**: If we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle.

* **Line styles** : 

There are several properties which allow us to style lines.

**lineWidth = value**
Sets the width of lines drawn in the future.

**lineCap = type**
Sets the appearance of the ends of lines.

**lineJoin = type**
Sets the appearance of the "corners" where lines meet.

**miterLimit = value**
Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.

**getLineDash()**
Returns the current line dash pattern array containing an even number of non-negative numbers.

**setLineDash(segments)**
Sets the current line dash pattern.

**lineDashOffset = value**
Specifies where to start a dash array on a line.

