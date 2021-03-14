A great way to get started with charts is with Chart.js, a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page. It’s a well documented plugin that makes using all kinds of bar charts, line charts, pie charts and more, incredibly easy.



Chart.js charts are rendered on user provided canvas elements. Thus, it is up to the user to create the canvas element in a way that is accessible. The canvas element has support in all browsers and will render on screen but the canvas content will not be accessible to screen readers.

With canvas, the accessibility has to be added with ARIA attributes on the canvas element or added using internal fallback content placed within the opening and closing canvas tags.



When it comes to changing the chart size based on the window size, a major limitation is that the canvas render size (canvas.width and .height) can not be expressed with relative values, contrary to the display size (canvas.style.width and .height). Furthermore, these sizes are independent from each other and thus the canvas render size does not adjust automatically based on the display size, making the rendering inaccurate.



By default the chart's canvas will use a 1:1 pixel ratio, unless the physical display has a higher pixel ratio (e.g. Retina displays).

For applications where a chart will be converted to a bitmap, or printed to a higher DPI medium it can be desirable to render the chart at a higher resolution than the default.

Setting devicePixelRatio to a value other than 1 will force the canvas size to be scaled by that amount, relative to the container size. There should be no visible difference on screen; the difference will only be visible when the image is zoomed or printed.


The hover configuration is passed into the options.hover namespace. The global hover configuration is at Chart.defaults.global.hover. To configure which events trigger chart interactions, see events.

When configuring interaction with the graph via hover or tooltips, a number of different modes are available.

Scriptable options also accept a function which is called for each of the underlying data values and that takes the unique argument context representing contextual informatio

When supplying colors to Chart options, you can use a number of formats. You can specify the color as a string in hexadecimal, RGB, or HSL notations. If a color is needed, but not specified, Chart.js will use the global default color. This color is stored at Chart.defaults.global.defaultColor. It is initially set to 'rgba(0, 0, 0, 0.1)'.


There are 4 special global settings that can change all of the fonts on the chart. These options are in Chart.defaults.global. The global font settings only apply when more specific options are not included in the config.


    canvas id="stockGraph" width="150" height="150"
      current stock price: $3.15 + 0.15
    /canvas

    canvas id="clock" width="150" height="150"
      img src="images/clock.png" width="150" height="150" alt=""/
    /canvas




As a consequence of the way fallback is provided, unlike the img element, the canvas element requires the closing tag (/canvas). If this tag is not present, the rest of the document would be considered the fallback content and wouldn't be displayed.




The canvas element creates a fixed-size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown. In this tutorial, we focus on the 2D rendering context. 


he fallback content is displayed in browsers which do not support canvas. Scripts can also check for support programmatically by testing for the presence of the getContext() method.




Unlike SVG, canvas only supports two primitive shapes: rectangles and paths (lists of points connected by lines). All other shapes must be created by combining one or more paths. Luckily, we have an assortment of path drawing functions which make it possible to compose very complex shapes.


Each of these three functions takes the same parameters. x and y specify the position on the canvas (relative to the origin) of the top-left corner of the rectangle. width and height provide the rectangle's size.




One very useful function, which doesn't actually draw anything but becomes part of the path list described above, is the moveTo() function. You can probably best think of this as lifting a pen or pencil from one spot on a piece of paper and placing it on the next.



This method takes two arguments, x and y, which are the coordinates of the line's end point. The starting point is dependent on previously drawn paths, where the end point of the previous path is the starting point for the following, etc. The starting point can also be changed by using the moveTo() method.


In this example, we are creating a rectangle and a circle. Both are stored as a Path2D object, so that they are available for later usage. With the new Path2D API, several methods got updated to optionally accept a Path2D object to use instead of the current path. Here, stroke and fill are used with a path argument to draw both objects onto the canvas, for example.



    function draw() {
      var canvas = document.getElementById('canvas');
      if (canvas.getContext) {
        var ctx = canvas.getContext('2d');

        var rectangle = new Path2D();
        rectangle.rect(10, 10, 50, 50);

        var circle = new Path2D();
        circle.arc(100, 35, 25, 0, 2 * Math.PI);

        ctx.stroke(rectangle);
        ctx.fill(circle);
      }
    }






In this example, we once again use two for loops to draw a grid of rectangles, each in a different color. The resulting image should look something like the screenshot. There is nothing too spectacular happening here. We use the two variables i and j to generate a unique RGB color for each square, and only modify the red and green values. The blue channel has a fixed value. By modifying the channels, you can generate all kinds of palettes. By increasing the steps, you can achieve something that looks like the color palettes Photoshop uses.




      function draw() {
        var ctx = document.getElementById('canvas').getContext('2d');
        for (var i = 0; i  6; i++) {
          for (var j = 0; j  6; j++) {
            ctx.fillStyle = 'rgb(' + Math.floor(255 - 42.5 * i) + ', ' +
                             Math.floor(255 - 42.5 * j) + ', 0)';
            ctx.fillRect(j * 25, i * 25, 25, 25);
          }
        }
      }




n addition to drawing opaque shapes to the canvas, we can also draw semi-transparent (or translucent) shapes. This is done by either setting the globalAlpha property or by assigning a semi-transparent color to the stroke and/or fill style.




In this second example, we do something similar to the one above, but instead of drawing circles on top of each other, I've drawn small rectangles with increasing opacity. Using rgba() gives you a little more control and flexibility because we can set the fill and stroke style individually.




      function draw() {
        var ctx = document.getElementById('canvas').getContext('2d');

        // Draw background
        ctx.fillStyle = 'rgb(255, 221, 0)';
        ctx.fillRect(0, 0, 150, 37.5);
        ctx.fillStyle = 'rgb(102, 204, 0)';
        ctx.fillRect(0, 37.5, 150, 37.5);
        ctx.fillStyle = 'rgb(0, 153, 255)';
        ctx.fillRect(0, 75, 150, 37.5);
        ctx.fillStyle = 'rgb(255, 51, 0)';
        ctx.fillRect(0, 112.5, 150, 37.5);

        // Draw semi transparent rectangles
        for (var i = 0; i  10; i++) {
          ctx.fillStyle = 'rgba(255, 255, 255, ' + (i + 1) / 10 + ')';
          for (var j = 0; j  4; j++) {
            ctx.fillRect(5 + i * 14, 5 + j * 37.5, 14, 27.5);
          }
        }


In the case you need to obtain more details about the text, the following method allows you to measure it.

      measureText()
      
      
Returns a TextMetrics object containing the width, in pixels, that the specified text will be when drawn in the current text style.
The following code snippet shows how you can measure a text and get its width.


    function draw() {
      var ctx = document.getElementById('canvas').getContext('2d');
      var text = ctx.measureText('foo'); // TextMetrics object
      text.width; // 16;
    }


LINKS USED:

1. https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/
2. http://www.chartjs.org/docs/
3. https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage
4. https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes
5. https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors
6. https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text





