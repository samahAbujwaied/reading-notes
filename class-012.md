# Drawing text 
![](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text/baselines.png)
### The canvas rendering context provides two methods to render text:

* fillText(text, x, y [, maxWidth])
*Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.*

##### A fill Text example
![](https://zetcode.com/img/gfx/html5canvas/drawing_text.png)

###### The text is filled using the current fillStyle.
   ```function draw() { var ctx = document.getElementById('canvas').getContext('2d'); ctx.font = '48px serif'; ctx.fillText('Hello world', 10, 50);}```

* strokeText(text, x, y [, maxWidth])
*Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.*
##### A stroke Text example
![](https://media.geeksforgeeks.org/wp-content/uploads/20190819143645/Screenshot-from-2019-08-19-14-36-07.png)

###### The text is filled using the current strokeStyle.
```function draw() {var ctx = document.getElementById('canvas').getContext('2d'); ctx.font = '48px serif'; ctx.strokeText('Hello world', 10, 50);}```

### Styling text
**In the examples above we are already making use of the font property to make the text a bit larger than the default size. There are some more properties which let you adjust the way the text gets displayed on the canvas:**
* font = value. 
  > The current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.
* textAlign = value
  > Text alignment setting. Possible values: start, end, left, right or center. The default value is start.
* textBaseline = value 
  > Baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.
* direction = value
  > Directionality. Possible values: ltr, rtl, inherit. The default value is inherit.

# Applying styles and colors 
![](http://i.stack.imgur.com/8Cdba.png)
 * Colors
  **If we want to apply colors to a shape, there are two important properties we can use:**
  1. fillStyle .
  2.  strokeStyle.
   *fillStyle = color*

**color is a string representing a CSS ```<color>```, a gradient object, or a pattern object. We'll look at gradient and pattern objects later. By default, the stroke and fill color are set to black (CSS color value #000000).**
   > Note: When you set the strokeStyle and/or fillStyle property, the new value becomes the default  for all shapes being drawn from then on. For every shape you want in a different color, you will need to reassign the fillStyle or strokeStyle property.
### A fill Style example
![](https://static.commonlounge.com/fp/600w/LZ1cBjfZz4U10BK1yyPieiWF11533914674_kc)
> ```function draw() { var ctx = document.getElementById('canvas').getContext('2d'); for (var i = 0; i < 6; i++) {  for (var j = 0; j < 6; j++) {  ctx.fillStyle = 'rgb(' + Math.floo (255 - 42.5 * i) + ', ' +        Math.floor(255 - 42.5 * j) + ', 0)';  ctx.fillRect(j * 25, i * 25 25, 25);  }  } }```

### A stroke Style example
![](https://media.prod.mdn.mozit.cloud/attachments/2012/07/09/253/c4e071f91f9aa7e0d29ff8696d37a27c/Canvas_strokestyle.png)
  > ```  function draw() { var ctx = document.getElementById('canvas').getContext('2d');  for (var i = 0; i < 6; i++) {  for (var j = 0; j < 6; j++) {   ctx.strokeStyle = 'rgb(0, ' + Math.floor(255 - 42.5 * i) + ', ' +  Math.floor(255 - 42.5 * j) + ')'; ctx.beginPath(); ctx.arc(12.5 + j * 25, 12.5 + i * 25, 10, 0, Math.PI * 2, true); ctx.stroke();}} }```

### Transparency
**In addition to drawing opaque shapes to the canvas, we can also draw semi-transparent (or translucent) shapes. This is done by either setting the globalAlpha property or by assigning a semi-transparent color to the stroke and/or fill style.**
 *globalAlpha = transparencyValue*

* A global Alpha example

![](https://static.commonlounge.com/fp/600w/J7xU2h1UYUVTJrIk5eOfld2ij1533914687_kc)

* An example using rgba()

![](https://media.prod.mdn.mozit.cloud/attachments/2012/07/09/246/258cf71b564f5bddb9e5180b567101b6/Canvas_rgba.png)

* A line Width example

![](https://media.prod.mdn.mozit.cloud/attachments/2012/07/09/239/7bdc0d7dffe1e887b327243c9c8687eb/Canvas_linewidth.png)

* A line Cap example 

![](http://i.stack.imgur.com/XwUuF.png)

* A line Join example

![](http://i.stack.imgur.com/XDrkB.png)

* A demo of the miterLimit property

![](https://media.prod.mdn.mozit.cloud/attachments/2012/07/09/240/1ef20a2b0f86279ce0e2f660d760eb7a/Canvas_miterlimit.png)

* Using line dashes

![](https://www.indezine.com/products/powerpoint/learn/fillslinesandeffects/images/outlineweightanddash_2007_04.gif)

* Gradients

![](https://css-tricks.com/wp-content/uploads/2021/02/gradient-borders-1.png)

* A create Radial Gradient example

![](https://static.commonlounge.com/fp/600w/xDGHtNhfAdxGxYrkCGzv2L6Yr1533916234_kc)

* A create Conic Gradient example 

![](https://i.stack.imgur.com/ATlVZ.gif)

* A create Pattern example

![](https://static.commonlounge.com/fp/600w/FQueni7qGBiganKB0U8t5pixQ1533916244_kc)

* A shadowed text example

![](https://codesdope-media.nyc3.cdn.digitaloceanspaces.com/prod/media/blog_images/15/2019/3/9/25shadow.png)

* Canvas fill rules

![](https://media.prod.mdn.mozit.cloud/attachments/2015/01/18/9855/c8d648daa8e6bd3d94756ee57b16a28d/fill-rule.png)

# Drawing shapes with canvas

* The grid

![](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes/canvas_default_grid.png)
 
#### Drawing rectangles
1. fillRect(x, y, width, height)
  **Draws a filled rectangle.**
2. strokeRect(x, y, width, height)
  **Draws a rectangular outline.**
3. clearRect(x, y, width, height)
  **Clears the specified rectangular area, making it fully transparent.**

* Rectangular shape example
![](https://media.prod.mdn.mozit.cloud/attachments/2012/07/09/245/abd4f1e1c012f5d3b636cd1b852b074c/Canvas_rect.png)
* Drawing paths
1. First, you create the path.
2. Then you use drawing commands to draw into the path.
3. Once the path has been created, you can stroke or fill the path to render it.

* beginPath() 
* Path methods
* closePath()
* stroke()
* fill()

##### Drawing a triangle 
![](https://media.prod.mdn.mozit.cloud/attachments/2015/01/18/9847/55a2b8b8e4ed4a33ffe023e5cbedb0a9/triangle.png)
##### Moving the pen
![](https://media.prod.mdn.mozit.cloud/attachments/2012/07/09/252/804dd546c6267e6391c4e3a87f922e33/Canvas_smiley.png)

##### Lines
![](https://media.prod.mdn.mozit.cloud/attachments/2012/07/09/238/80b2d1ec2c598631e8ac9cffe494b2d9/Canvas_lineTo.png)
##### Arcs
![](https://media.prod.mdn.mozit.cloud/attachments/2012/07/09/204/370c33c99436bb42b3b7b547dec13b72/Canvas_arc.png)
##### Quadratic Bezier curves
![](https://media.prod.mdn.mozit.cloud/attachments/2012/07/09/243/b1ae318387b382e74b674cf80ea728f8/Canvas_quadratic.png)
##### Cubic Bezier curves
![](https://media.prod.mdn.mozit.cloud/attachments/2012/07/09/207/0954a1e75abbc138907c58314849938a/Canvas_bezier.png)
##### Rectangles (Making combinations)
![](https://media.prod.mdn.mozit.cloud/attachments/2015/01/18/9849/58c451f48da1af60cf343f83daf9f25b/combinations.png)
##### Path2D example 
![](https://media.prod.mdn.mozit.cloud/attachments/2015/01/18/9851/2a2e7589207b3967d48c3ea929561efc/path2d.png)

# Basic usage of canvas

![](https://www.webfx.com/blog/images/assets/images.sixrevisions.com/2010/10/03-01_html5_canvas_element_ld_img.png)

* The ```<canvas>``` element
* The rendering context
* Checking for support
* A skeleton template
###### A skeleton template
![](https://media.prod.mdn.mozit.cloud/attachments/2012/07/09/228/0bed6a3ebfcc9d739a3a9fbc4de856f3/canvas_ex1.png)


