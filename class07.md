# Read: 07 - HTML Tables; JS Constructor Functions
## Domain Modeling
Domain modeling is the process of creating a conceptual model in code for a specific problem.

A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders.

## Define a constructor and initialize properties
To define the same properties between many objects, you'll want to use a constructor function. 
**constructor function.**
Example:
```
var EpicFailVideo = function(epicRating, hasAnimals) {
  this.epicRating = epicRating;
  this.hasAnimals = hasAnimals;
}

var parkourFail = new EpicFailVideo(7, false);
var corgiFail = new EpicFailVideo(4, true);
```

constructor function is defined using a function expression. In other words,then assigned a function with the parameters.
When the function is called, the data inside these parameters are stored inside the this.Storing data within properties ensures any newly created object can access that data later.

After the constructor function definition,*objects* are instantiated with the **new keyword** and their properties are initialized by calling the constructor function. 

## Generate random numbers

JavaScript standard library includes a Math.random() function for just this sort of occasion.

----
## HTML Tables
A table represents information in a grid format. 
Grids allow us to understand complex data by referencing information on two axes

The ```<table>``` element is used to create a **table**. The contents of the table are written out *row by row*.
```<tr>```You indicate the start of each row using the opening tr tag. (The tr stands for **table row.**) It is followed by one or more ```<td>``` elements (**one for each cell** in that row).
At the end of the row you use a closing tr tag.

![table](https://vertex-academy.com/tutorials/wp-content/uploads/2016/08/table.png)

👉
*Note* 

The <th> element is used just like the <td> element but its purpose is to represent the heading for either a column or a row. (The th stands for table
heading.) 

### Spanning ColumnS & Spanning Rows
The colspan & rowspan attribute can be used on a ```<th> or <td>``` element and indicates how many columns that cell should run across or  how many rows a cell should span down the table.

![span](https://i.stack.imgur.com/Uvzmu.jpg)

### Long Tables
There are three elements that help distinguish between the main content of the table and the first and last rows.
1. ```<thead>``` The headings of the table should
sit inside the thead element. 
2. ```<tbody>``` The body should sit inside the
tbody element. 
3. ```<tfoot>``` The footer belongs inside the
<tfoot> element.

#### Why Long Tables?!
These elements help people who use screen readers and also allow you to style these sections
in a different manner than the rest of the table (as you will see when you learn about CSS).


## Constructor Functions(JS)


### Updating An Object
* dot notation 
```
 ObjectName . PropertyName = 'value';
 ```
* square bracets
``` 
ObjectName[ 'PropertyName'] = 'value';
```

### Creating Many Objects
several objects represent similar things.
Object constructors can use a function as a template for creating objects.

* First, create the template with the object's properties and methods. 
* A function will be used as a template for creating new objects.they add properties or methods to the object. 
* The new keyword followed by a call to function creates a new object.


### Creating Object
* LITERAL NOTATION

* OBJECT CONSTRUCTOR NOTATION 

![Cobj](https://i0.wp.com/miro.medium.com/max/4096/1*KYFTHD69xtacnwbKRyFuqQ.png)

👉
*Notes* 


-Once you have created an object, the syntax for adding or removing any properties and methods from that object is the same. 

-The keyword **this** is commonly used inside functions and objects.
Where the function is declared alters what this means. It always refers
to one object, usually the object in which the function operates. 


### ADDING AND REMOVING PROPERTIES
Once you have created an object (using literal or constructor notation), you can *add new properties* to it.
You do this using the **dot notation**.
To *delete a property*, you use the keyword **delete**, and then use dot notation to identify the
property or method you want to remove from the object. 
Example:
```
hotel .pool = fal se;
delete hotel .booked; 
```

### STORING DATA
* **VARIABLES** A variable has just one key (the variable name) and **one value**. 
* **ARRAYS** Arrays can store **multiple** pieces of information.Each piece of information is separated by a *comma*.The order of the values is important because items in an array are assigned a number (called an *index*). 

### WHAT ARE BUILT-IN OBJECTS? 
Browsers come with a set of built-in objects that represent things like the
browser window and the current web page shown in that window. These
built-in objects act like a toolkit for creating interactive web pages.

* Browser Object Model
![BOM](https://static.javatpoint.com/images/javascript/bom.jpg)
 is used to interact with the browser.

The default object of browser is window means you can call all the functions of window by specifying window or directly. For example:
``` 
window.alert("hello javatpoint");
 ```

is same as:

```
alert("hello javatpoint");
  ```

* Document Object Model
![DOM](https://www.researchgate.net/profile/Henrique-Gaspar/publication/317624714/figure/fig10/AS:668885598605336@1536486162639/HTML-Document-Object-Model-DOM-three-of-objects.png)
 represents the whole html document.

When html document is loaded in the browser, it becomes a document object. It is the root element that represents the html document. It has properties and methods. By the help of document object, we can add dynamic content to our web page.

``` 
window.document 
```

Is same as

```
document 
```

### GLOBAL OBJECTS: DATE OBJECT (AND TIME)

Once you have created a **Date object,** the following methods let you set and retrieve the time and date that it represents.

![GO/Date](https://1.bp.blogspot.com/-Y2DObhTLxr0/W7kDOsuhXNI/AAAAAAAAEtw/gwNKf10REIcm9NhzjkN2VSlyE8ikR8MhgCLcBGAs/s640/DownloadFile%2B%25281%2529.png) 
