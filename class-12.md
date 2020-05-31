# Docs for the HTML **canvas** Element & Chart.js
The charts are more better than tables to display data in visual.

**There are 3 types of charts, and they are:**
- Line chart
- pie chart
- Bar chart

**Canvas** element has 2 attributes (**width** and **height**)

**To draw a rectangles there are 3 functions on canvas elemnts:**
- fillRect(x, y, width, height)
- strokeRect(x, y, width, height)
- clearRect(x, y, width, height)
**To draw a paths there are 4 functions on canvas elemnts:**
- beginPath()
- closePath()
- stroke()
- fill()
**To apply colors to a shape, there are two important properties we can use:** 
- fillStyle = color
- strokeStyle = color
We can  draw semi-transparent shapes by **globalAlpha = transparencyValue**
**To style lines there are several properties:**
- lineWidth = value
- lineCap = type
- lineJoin = type
- miterLimit = value
- getLineDash()
- setLineDash(segments)
- lineDashOffset = value
**We can fill and stroke shapes using linear and radial gradients.**
**To create a pattern of images we can use createPattern(image, type) method.**
**The type specifies how to use the image in order to create the pattern, and must be one of the following string values:**
- repeat
- repeat-x
- repeat-y
- no-repeat
**Shadows involves just four properties:**
- shadowOffsetX = float
- shadowOffsetY = float
- shadowBlur = float
- shadowColor = color
**There are 2 methods to render text:**
- fillText(text, x, y [, maxWidth])
- strokeText(text, x, y [, maxWidth])
**The way of displaying the text on the canvas:**
- font = value
- textAlign = value
- textBaseline = value
- direction = value
**When we need to obtain more details about the text, measureText() method allows us to measure it.**
[Main Page](https://basma23.github.io/reading-notes/)
