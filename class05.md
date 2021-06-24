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

## HTML TEXT
### Typeface Terminology
Typefaces are subject to copyright, so the techniques you can choose from are limited by their respective licenses.
Typefaces Examples:
* Serif
* Sans-Serif
* Monospace

-The ***font-family*** property allows you to specify the typeface that should be used for any text inside the element(s) to which a CSS rule applies.

-The ***font-size*** property enables you to specify a size for the font. There are several ways to specify the size of a font.
The most common are:
* *pixels* The default size of text in browsers is 16px. 
* *percentages* A size of 75% would be the equivalent of 12px, and 200% would be 32px.
* *ems* An em is equivalent to the widthof a letter m.

-***@font-face*** allows you to use a font, even if it is not installed on the computer of the person browsing.

-***font-weight*** allows you to create bold text.There are two values that this
property commonly takes: *normal* This causes text to appear at a normal weight.
*bold* This causes text to appear bold.

-***font-style** There are three values this property can take:
*normal* This causes text to appear in a normal style (as opposed to italic
or oblique). *italic* This causes text to appear italic. *oblique* This causes text to appear oblique.

-***text-transform*** Is used to change the case of text giving it one of the following values: *uppercase* This causes the text to appear uppercase.
*lowercase* This causes the text to appear lowercase. *capitalize* This causes the first letter of each word to appear capitalized.

-***text-decoration*** ِllows you to specify the following values:
*none* This removes any decoration already applied to the text.
*underline* This adds a line underneath the text.
*overline* This adds a line over the top of the text.
*line-through* This adds a line through words.
*blink*  This animates the text to make it flash on and off (however this is
generally frowned upon, as it is considered rather annoying).

-***line-height*** Sets the height of an entire line of text.

-***letter-spacing*** control the space between each letter(Kerning).

-***text-align*** Allows you to control the alignment oftext. The property can take one of four values:
*left* This indicates that the text should be left-aligned.
*right* This indicates that the text should be right-aligned.
*center* This allows you to center text.
*justify* This indicates that every line in a paragraph, except the last line,
should be set to take up the full width of the containing box.

-***vertical-align*** Sets the vertical alignment of an element.

-***text-indent*** Specifies the indentation of the first line in a text-block.

-***text-shadow*** Adds shadow to text.

-You can specify different values for the first letter or first line of text inside an element using ***:first-letter*** and ***:first-line.***


### Styling Links 

Browsers tend to show links in blue with an underline by default, and they will change the color of links that have been visited to help users know which pages they have been to.

-***:link*** This allows you to set styles for links that have not yet been
visited.
-***:visited*** This allows you to set styles for links that have been clicked on.

-Three pseudo-classes that allow you to change the appearance of elements when a
user is interacting with them.
* *:hover* This is applied when a user hovers over an element with a
pointing device such as a mouse.
* *:active* This is applied when an element is being activated by a user; for
example, when a button is being pressed or a link being clicked.
* *:focus* This is applied when an element has focus. Any element that
you can interact with, such as alink you can click on or any form control can have focus.

----
## JPEG vs PNG vs GIF — which image format to use and when?

There are hundreds of image formats available, we would only be looking at the three *most commonly used* image formats, these 3 image formats have *significant differences* amongst themselves thus making each of them suitable for specific use cases. 

* **JPEG** use for all images that contain a natural scene or photograph where variation in colour and intensity is smooth.
* **PNG** use for any image that needs transparency or for images with text & objects with sharp contrast edges like logos.
* **GIF** use for images that contain animations.

### Compression
Almost all forms of data that we see on the internet — text, image, video etc. — are compressed to **reduce the size** of data and ensure **faster**.

Compression can be of two types:
* **lossless** In lossless compression, it is possible to reconstruct the original image from the compressed image because there is no information loss during compression. 
* **lossy** Data loss in lossy compression is irreversible. 


### Transparency
In a simple form, transparency indicates something that is completely invisible. 
**JPEG** images ~~don’t support~~ transparency and are hence not usable for such cases.
**PNG** images support transparency. 
**GIF** images support transparency.

### Colours
There is a significant difference in the number of colours that can be supported by these 3 formats.
**JPEG** images can support around 16 million colours. This is what makes them suitable for storing images of natural scenes.
**PNG** images mainly have two modes — PNG8 and PNG24. PNG8 can support upto 256 colours whereas PNG24 can handle upto 16 million colours like a JPEG image. Use PNG8 for simple shapes with fewer colours and PNG24 for high quality, complex logos and shapes with rounded corners on a transparent background.
**GIF** images are limited to 256 colours. If index transparency is used, then one of these 256 colours is assigned as transparent and the remaining 255 are used for other colours.

### Animation
Animation, in this case, refers to any change or movement in the image.
Of these 3 formats, **only GIF** supports animation.