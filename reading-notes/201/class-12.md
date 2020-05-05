# Charts
To display data, use the chart.js plugin by importing the minified file into your code using the script tag.  View the [documentation](https://www.chartjs.org/docs/latest/) or see [examples](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/) 

# Canvas
The `canvas` element is used for displaying graphics.  It creates a fixed-sized drawing surface and is a *container* for the graphics and therefore CSS doesnt apply to the actual graphic itself. 

Unlike `<img>` or `<video>`, the `<canvas>` element requires a closing tag (`</canvas>`)

To draw on the canvas, you use the canvas grid or **coordinate space**: ![canvas](./images/canvas.png)

Canvas only supports two primative shapes: rectangles and paths (list of points connected by lines)

The functions used to draw rectangles in `canvas`:
1. `fillRect(x, y, width, height)`: draws a filled rectangle
2. `strokeRect(x, y, width, height)`: draws a rectangle outline
3. `clearRect(x, y, width, height)`: makes the rectangle transparent 
4. `rect(x, y, width, height)`: draws a rectangle whose top-left corner is at the x,y coordinate

The functions used to draw a path: 
1. `beginPath()`: creates a new path
2. `closePath()`: adds a straight line to the path
3. `stroke()`: strokes the outline
4. `fill()`: fills the path's content area
5. `moveTo(x, y)`: moves the path to a different area (think of lifting the pen off the paper)

To draw arcs or circles you use the following methods: 
1. `arc(x, y, radius, startAngle, endAngle, anticlockwise)`: draws an arc centered at x,y
2. `arcTo(x1, y1, x2, y2, radius)`: draws an arc connected to the previous point by a line


To draw text, you can use `fillText` or `strokeText` and style it using `fillStyle` or `strokeStyle`
