## Chart.js, canvas

**Chart.js** is a JavaScript plugin that uses HTML5's canvas element to draw the chart on the page.

Drawing a line chart:
- create a canvas element in HTML
- write script to retrieve chart content
- create data

Canvas Element:
`<canvas id="tutorial" width="150" height="150"></canvas>`
- can be styled just like any normal image
- provide fallback content to be displayed in older browsers
- unlike image requires a closing tag
- rendering contxts: create and manipulate the content shown
- `getContext()` takes in a parameter of the type of context and is used to  obtain the rendering context
  - can also use this method to check for browser support

The Grid:
- canvas grid or coordinate space
- all elements placed relative to the origin
example rectangle code:
`function draw() {
  var canvas = document.getElementById('canvas');
  if (canvas.getContext) {
    var ctx = canvas.getContext('2d');

    ctx.fillRect(25, 25, 100, 100);
    ctx.clearRect(45, 45, 60, 60);
    ctx.strokeRect(50, 50, 50, 50);
  }
}`

Creating paths:
- `beginPath()` starts the drawing path
- `closePath()` adds a straight line to the path
- `stroke()` draws a shape by stroking its outline
- `fill()` fills the current shape
- `move(x,y)` moves the pen to x and y without making marks
- `lineTo(x,y)` draws a line from current position to x,y
- `arc(x, y, radius, startAngle, endAngle, anticlockwise)` draws an arc centered at x,y. determines arc's radius, angle, and whether its clockwise or counter clockwise

Color: 
- `fillstyle = color` fills with color
- `strokestyle = color` changes color of stroke
- transparancy: `globalAlpha: transparancyValue` sets value between 0.0 (transparent) and 1.0 (opaque)

Line Styles:
- `lineWidth = value` sets width
- `lineCap = type` sets appearance of the end of the lines
- `lineJoin = type` sets appearance of corners where lines meet
- `masterLimit = value` controls thickenss of junctions of two joining lines
- `getLineDash()` returns the current line dash pattern array
- `setLineDash(segments)` sets current line dash pattern
- `lineDashOffset = value` specifies where to start a dash array on a line

Gradients:
- `createLinearGradient(x1,y1,x2,y2)` creates a linear gradient object with a start and end point
- `createRadialGradient(x1,y1,r1,x2,y2,r2)` creates a radial gradient based on two circles

Patterns:
- `createPattern(image, type)` creates and returns a new canvas pattern object
- type specifies how to use the image to create a pattern, can be: repeat, repeat-x, repeat-y, no-repeat

Shadows:
- `shadowOffsetX = float` indicates horizontal distance the shadow should extend from the object
- `shadowOffsetY = float` indicates horizontal distance the shadow should extend from the object
- `shadowBlur = float` indicates size of blurring effect
- `shadowColor = color` determines color of shadow

Text:
- `fillText(text, x, y [, maxwidth])` fills a given text at x,y position
- `strokeText(text, x, y [, maxWidth])` strokes a given text at x,y position

Styling text:
- `font = value`
- `text-align = value`
- `text-baseline = value`
- `direction = value`
