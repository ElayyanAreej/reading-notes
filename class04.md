# Read: 04 - HTML Links, CSS Layout, JS Functions
## HTML Links
Links allow you to move from one web page to another.

Links are created using the ``` <a> ``` element. Users can click on anything between the opening ``` <a> ``` tag and the closing ``` </a> ``` tag. You specify which page you want to link to using the *href* attribute.

![a](https://i0.wp.com/learnwebanalytics.com/wp-content/uploads/2018/12/What-Is-An-Anchor-Tag.png?fit=1211%2C501&ssl=1)

👉
*Notes* 

-An **absolute URL** starts with the domain name for that site, and can be followed by the path to a specific page.

-When you are linking to other pages within the same site, you do not need to specify the domain name in the URL. You can use a shorthand known as a **relative URL**.

### Directory Structure

On larger websites it's a good idea to organize your code by placing the pages for each different section of the site into a new folder. *Folders* on a website are sometimes referred to as *directories*.

👉
*Notes* 

-The top-level folder is known as the **root folder**.

-The main homepage of a site written in HTML (and the homepages of each section in a child folder) is called **index.html**.

-If all of the files in your site are in one folder, you simply use the
file name for that page.

-If your site is organized into separate folders (or directories), you need to tell the browser how to get from the page it is currently on to the page that you
are linking to.

-To create a link that starts up the user's **email** program this time the
value of the *href* attribute starts with *mailto:* and is followed by
the email address you want the email to be sent to.

-**target** attribute Specifies where to open the linked document.*_blank*	Opens the linked document in a new window or tab.
```
<a target="_blank|_self|_parent|_top|framename">
```
###  link To A Specific Part Of The Same Page
You can link to a specific part of a page, you need to identify the *points* in the page that the link will go to.You do this using the *id attribute* (which
can be used on every HTML element).

```
<h2 id="C4">Chapter 4</h2>
// Then
<a href="#C4">Jump to Chapter 4</a>
```

###  link To A Specific Part Of Another Page
f you want to link to a specific part of a different page (whether on your own site or a different website) you can use a similar technique.
```
<a href="html_demo.html#C4">Jump to Chapter 4</a>
```

```
<a href="http:/www.htmlandcssbookcom/#bottom">
```
## HTML Layout
Websites often display content in multiple columns.

### Building Blocks
CSS treats each HTML element as if it is in its own box. This box will either be a **block-level** box(start on a new line) or an **inline** box (flow in between
surrounding text).

### Containing Elements
If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.

### position:
The ***position property*** specifies the type of positioning method used for an element (static, relative, fixed, absolute or sticky).

* **static**
positioned according to the normal flow of the page,in normal flow each block-level element sits on top of the next one(this is the default).

* **relative**
 positioned relative to its normal position.

* **fixed**
positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled.

* **absolute**
positioned relative to the nearest positioned ancestor (instead of positioned relative to the viewport, like fixed).

* **sticky**
positioned based on the user's scroll position.

👉
*Note* 
When elements are positioned, they can overlap other elements.
The **z-index** property specifies the stack order of an element (which element should be placed in front of, or behind, the others).
**Its value is a number, and the higher the number the closer that element
is to the front.**

### Floating Elements
The float property allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible.

👉
*Note* 

When you use the float property, you should also use the *width* property to indicate how wide the floated element should be.

### Clearing Floats
The **clear** property allows you to say that no element (within the same containing element) should touch the left or righthand sides of a box.
* *left* The left-hand side of the boxshould not touch any other elements appearing in the same containing element.

* *right* The right-hand side of the box will not touch elements
appearing in the same containing element.

* *both*  Neither the left nor right-hand sides of the box will touch elements appearing in the same containing element.

* *none* Elements can touch either side.


👉
*Note*

Different visitors to your site will have different sized screens that show
different amounts of information, so your design needs to be able to
work on a range of different sized screens.

## Functions

Functions let you group a series of statements together to perform a
specific task. If different parts of a script repeat the same task, you can
reuse the function (rather than repeating the same set of statements). 

![func](https://cdn.programiz.com/cdn/farfuture/NdxxeWlRfoHMPgdcWPkeVy1wN9MwAgoqoYqZkFQDMFQ/mtime:1591592059/sites/tutorial2program/files/javascript-function-example1.png)

Function need information:
![func2](https://cdn.programiz.com/cdn/farfuture/oAZVf3IqOKOYj_aJ-IoYQvbJ2CB-B3y4HXSLXBUmYcY/mtime:1591592163/sites/tutorial2program/files/javascript-function-with-parameter.png)

* Get Single Value Out Of A Function:
```
let x= FunctionName(argumates , , );
```

-----
* Get Multiple Values Out Of A Function:
Function returnes an array
```
let x= FunctionName(argumates , , )[0];
```
You can repet it over all indexes.

👉
*Note*

The location where you declare a variable will affect where it can be used
within your code. If you declare it within a function, it can only be used
within that function. This is known as the variable's scope.
* **LOCAL VARIABLES**
* **GLOBAL VARIABLES** 
