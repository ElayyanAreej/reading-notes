# Read: 09 - Forms and Events
## Forms HTML
![form](https://miro.medium.com/max/2560/1*EwtDrkuz9KfJYUSFc4Xm4g.png)
### Why ?
Enabling users to search, forms also allow users to perform other functions online.ex(when registering as a member of a website, when shopping online, and when signing up for newsletters or mailing lists.

### Form Controls
* ADDING TEXT:
  + Text input (single-line)
   + Password input
   + Text area (multi-line)

* Making Choices:
    * Checkboxes
    * Radio buttons
    * Drop-down boxes
* Submitting Forms:
   * Submit buttons
   * Image buttons
* Uploading Files:

### How Forms Work ?
A user fills in a form and then resses button to submit the information to the server.

**The name of each form control is sent to the server along with the
value the user enters or selects.**

### Form Structure
```<form>```
This element should always carry the ***action*** attribute ( Its value is the URL for the page on the server that will receive the information in the form when it is submitted) and will usually have a ***method*** and id attribute too.

* ```<input>```
   + **Text** input (single-line)
   ```
    <input type="text"   ....>
   ```
   + **Password** input just like a single-line text input, except the characters are blocked out. They are hidden in this way so that if omeone is looking over the user's shoulder, they cannot see sensitive data.
   ```
    <input type="password"   ....>
   ```
   + **Radio button** allow users to pick just one of a number of options.
   ```
   <input type="radio"   ....>
   ```
   + **checkbox** allow users to select
   (and unselect) one or more options in answer to a question.
   ```
   <input type="checkbox"   ...>
   ```
   + **File** Input Box allow users to upload a file.
   ```
   <input type="file"   ...>
   ```
   + **submit button** The submit button is used to send a form to the server.
   ```
   <input type="submit"   ...>
   ```
   + **Image Button** to use an image for the submit button.
   ```
   <input type="image" src="images/subscribe.pg"  width="100" height="20" />
  ```
  + **Date**
  ```
   <input type="date"   ...>
   ```
  + **Email**
  ```
   <input type="email"   ...>
   ```
  + **URL**
   ```
   <input type="url"   ...>
   ```
   + **Search**
   ```
   <input type="search"   ...>
   ```

*  ```<textarea>```
**Text area** (multi-line)

* ```<select>``` ``` <option>```
**Drop Down List Box** allows users to select one option from a drop down list.

* ```<button>``` allow users more control over how their buttons appear, and to allow other elements to appear inside the button.

* ```<label>``` When introducing form controls,
the code was kept simple by indicating the purpose of each one in text next to it. 

#### Grouping Form Elements

You can group related form controls together inside the ```<fieldset>``` element. 

Most browsers will show the fieldset with a line around the edge to show how they arerelated.

The ```<legend>``` element can come directly after the opening fieldset tag and contains a caption which helps identify the purpose of that group of form controls.

## List CSS
The ***list-style-type*** property allows you to control the shape or style of a bullet point (also known as a marker).

For an unordered list you can use
the following values:
 - none
 - disc
 - circle
 - square

For an ordered (numbered) list you can use the following values:
- decimal
1 2 3
- decimal-leading-zero
01 02 03
- lower-alpha
a b c
- upper-alpha
A B C
- lower-roman
i. ii. iii.
- upper-roman  I II III

You can specify an image to act as a bullet point using the ***list-style-image*** property.

***list-style-position*** This property can take one of two values:
* outside

The marker sits to the left of the
block of text. (This is the default
behaviour if this property is not
used.)
* inside

The marker sits inside the box of
text (which is indented)

## Table CSS
### Table Properties
* *width* to set the width of the table.
* *padding* to set the space between the border of each table cell and its content.
* *text-transform* to convert the content of the table eaders to.
* *uppercase* letter-spacing, font-size to add additional styling to the content of the table headers
* *border-top, border-bottom* to set borders above and below the table headers.
* *text-align* to align the writing to the left of some table cells and to the right of the others.
* *background-color* to change the background color of the alternating table rows.
* *:hover* to highlight a table row when a user's mouse goes over it.

### Styling Forms
* *font-size* sets the size of the text entered by the user.
* *color* sets the text color, and *background-color* sets the background color of the input.
* *border* adds a border around the edge of the input box, and *border-radius* can be used to create rounded corners (for browsers that support this property).
* The *:focus* pseudo-class is used to change the background color of the text input when it is being used, and the *:hover* psuedo-class applies the same
styles when the user hovers over them.
* *background-image* adds a background image to the box.

### Cursor Style
cursor property allows you to control the type of mouse
cursor that should be displayed to users.
The most commonly used values for this property:
* auto
* crosshair
* default
* pointer
* move
* text
* wait
* help
* url("cursor.gif");