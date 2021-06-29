# Read: 08 - More CSS Layout
## Layout
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
