# Read: 05 - HTML Images; CSS Color & Text
## HTML Images
To add an image into the page
you need to use an ``` <img> ``` element. This is an empty element (which means there is no closing tag). It must carry the following two attributes:
* *src*
This tells the browser where it can find the image file.
* *alt* This provides a text description of the image which describes the image if you cannot see it.
* *title* To provide additional information about the image. when hovers over the image.

Use two other attributes that specify its size:
* *height* This specifies the height of the image in pixels.
* *width* This specifies the width of theimage in pixels.

👉
*Note* 

*align* cattribute was commonly used to indicate how the other parts of a page should flow around an image. It has been removed from HTML5 and new websites should use CSS to control the alignment of images

The ```<figcaption>``` element has been added to HTML5 in order to allow web page authors to add a caption to an image.

## CSS Color
The color property allows you to specify the color of text inside an element. You can specify any color in CSS in one of three ways:
* **rgb values**
These express colors in terms of how much red, green and blue are used to make it up. For example: rgb(100,100,90)

* **hex codes**
These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign. For example: #ee3e80

* **color names**
There are 147 predefined color names that are recognized by browsers. For example:
DarkCyan


-*background-color*
CSS treats each HTML element as if it appears in a box, and the background-color property sets the color of the background for that box.

-**Hue** is near to the colloquial idea of color. Technically speaking
however, a color can also have **saturation** and **brightness** as
well as hue.

*Saturation* refers to the amount of gray in a color. At maximum saturation, there would be no gray in the color. At minimum saturation, the color would be mostly gray.
*Brightness* ("value") refers to how much black is in a color. At maximum brightness, there would be no black in the color. At minimum brightness, the
color would be very dark.
![HSB](https://i.stack.imgur.com/PvK4n.png)

#### opacity, rgba
CSS3 introduces the opacity property which allows you to specify the opacity of an element and any of its child elements.
The value is a number between 0.0 and 1.0 (so a value of 0.5 is 50% opacity and 0.15 is 15% opacity).

#### HSL Color
way to specify colors using hue, saturation, and lightness values.

#### HSLA Color
alpha This is expressed as a number between 0 and 1.0.
For example, 0.5 represents 50% transparency, and 0.75 represents 75% transparency.

## Read About [HTML TEXT](class02.md)