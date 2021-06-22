# Read: 02 - HTML Text, CSS Introduction, and Basic JavaScript Instructions
## HTML Text 
### Headings
HTML has six "levels" of headings:
```
<h1>This is a Main Heading</h1>
<h2>This is a Level 2 Heading</h2>
<h3>This is a Level 3 Heading</h3>
<h4>This is a Level 4 Heading</h4>
<h5>This is a Level 5 Heading</h5>
<h6>This is a Level 6 Heading</h6>
```
![heading](https://www.tutorialrepublic.com/lib/images/html/html-headings.png)

## Paragraphs
To create a paragraph, surround the words that make up the paragraph with an opening ``` <p> ``` tag and closing ``` </p> ``` tag.

👉
*Notes* 
- By default, a browser will show each paragraph on a new line.

- ```<b>``` By enclosing words in the tag b can make characters appear **bold**.

- ``` <i> ``` By enclosing words in the tag i can make characters appear **italic**.

- ``` <sup> ``` is used
to contain characters that
should be superscript.

- ``` <sub> ``` is used to
contain characters that should
be subscript. 

- **White Space**  In order to make code easier to read, web page authors often add extra spaces or start some elements on new lines.

- ``` <br> ``` to add a line break inside the middle of a paragraph.

- ``` <hr> ``` to add a horizontal rule between sections.

### Semantic Markup
There are some text elements that are ot intended to affect the structure of your web pages, but they do add extra information to the pages — they are known as semantic markup.

- ``` <strong> ``` to indicates that its content has strong importance.

- ``` <em> ``` to indicates emphasis that subtly changes the meaning of a sentence.

- ``` <blockquote> ``` used for longer quotes that take up an entire paragraph. & ``` <q> ```  used for shorter quotes that sit within
a paragraph. 

- ``` <abbr> ``` 
![](https://www.android-examples.com/wp-content/uploads/2016/03/abbr-tag.png)

- ``` <cite> ``` to indicate where the citation is from.

- ``` <dfn> ```  to indicate the defining instance of a new term.

- ``` <address> ```  to contain contact details for the author of the page.

- ``` <ins> ``` to show content that has been inserted into a document, ``` <del> ```  show text that has been deleted from it.
![ins & dell](https://qph.fs.quoracdn.net/main-qimg-203ec72a9d01b698d726b0b6e9a73476)

- ``` <s> ```  indicates something that is no longer accurate or relevant (but that should not be deleted).

## CSS 
CSS allows you to create rules that specify how the content of an element should appear.

CSS allows you to create rules that control the way that each individual box (and the contents of that box) is presented.

![css](https://martinblackburn.co.uk/posts/2019-03-21-anatomy-of-a-css-rule/css-rule.png)


## Three Ways to Insert CSS:
![](https://wholeblogs.com/wp-content/uploads/2021/03/imageof3-1-1.jpg)
1. **Inline CSS**: defined within the "style" attribute of the relevant element.

2. **Internal CSS** : defined within the "style" element, inside the "head" section of an HTML page. 

3.**External CSS** :
defined within the "link" element, inside the "head" section of an HTML page

Use three attributes:
* **href** This specifies the path to the CSS file (which is often placed in
a folder called css or styles).

* **type** This attribute specifies the type of document being linked to. The
value should be text/css.
* **rel** This specifies the relationship between the HTML page and the file it is linked to. The value should be stylesheet.

## JavaScript
A script is a series of instructions that a computer can follow one-by-one.
Each individual instruction or step is known as a statement.
Statements should end with a semicolon. 
Each code block could contain many more statements

👉
*Note*

JAVASCRIPT IS CASE SENSITIVE 

**Comments** to explain what your code does.
They help make your code easier to read and understand.
This can help you and others who read your code. 

```
/* multi-line comment */
```
```
// single-line comment
```

**Variables**
Temporarily store the bits of information it needs to do its job.
with the keyword **let (or var) or const** followed by a name for your variable.
const keyword to define a variable that cannot be reassigned,and the let keyword to define a variable with restricted scope.

```
var variableName = num or string or boolean value;
```
#### Declare Variables
```
var variableName;
```
#### Assign Value
```
variableName = value ;
```

### DATA TYPES 

* Numeric data type handles numbers. 
* Strings data type consists of letters and other characters. 
* Boolean data types can have one of two values: true or false. 


👉
*Notes*

- String is placed inside quote marks. The quotes can be single or double quotes, but they must match and strings must always be written on one line.

- Because strings can live in single or double quotes, if you just want to use double quotes in the string, you could surround the entire string in single quotes. 


- Once you have assigned a value to a variable, you can then change what is stored in the variable later in the same script. 


### Shorthand To Create Variables
Variables are declared andvalues assigned in the same statement. 
Example 
```
var price = 5 , quantity = 14; 
```

### Rules For Naming 

- Remember that JavaScript identifiers (names) must begin with:
  - A letter (A-Z or a-z)
  - A dollar sign ($)
  - Or an underscore (_)
  - Not startwith a ~~number~~. 
- The name can contain letters, numbers, dollar sign ($), or an underscore (_). Note that you must not use a ~~dash(-) or a period (.)~~ in a variable name. 
- You ***cannot use keywords*** or reserved words.
- All variables are ***case sensitive***.
- Use a name that describes the kind of information that the variable stores.
- f your variable name is made up of more than one word, use a
capital letter for the first letter of every word after the first word.
For example, f i rstName rather than fi rstnarne (this is referred
to as ***camel case***.


## Condition (Decision making)
 A conditional code block allows you to run code selectively, depending on whether a certain condition is true or not. conditional block starts with the **keyword if**, then some parentheses, then some curly braces. Inside the parentheses we include a test. If the test returns true, we run the code inside the curly braces. If not, we don't, and move on to the next bit of code.
 ```
 if(test){
   // True case code;
 }
 else {
  // False case code;
 }
 ```
 ![h](https://craftofcoding.files.wordpress.com/2020/04/controlstr_if1.jpg)

### comparison operator
A **comparison operator** compares its operands and returns a logical value based on whether the comparison is true.

| Operator    | Name                  |
| ----------- | -----------           |
|    ==       | Equal                 |  
|    !=       | Not equal             |  
|    ===      | Strict equality       |  
|    !==      | Non-equality          |
|     <       | Less than	          |
|     >       | Greater than          |
|     >=      | Greater than or equal |
|     <=      | Less than or equal    |

👉
*Notes* 

- Strict equality returns true if the operands are equal and of the same type.
- You can evaluate two variables using a comparison operator to return a true or false value. 
```
var pass = 50; II Pass mark
var score = 90; II Score
II Check if t he user has passed
var hasPassed = score >= pass; 
```

### **Logical operators**

Logical operators are typically used with **Boolean** (logical) values; when they are, they return a Boolean value. 


 *Logical AND* **&&** returns true if both operands are true,otherwise returns false.

 *Logical OR* **||** returns true if either operand is true; if both are false, returns false.

 *Logical NOT* **!** returns false if its single operand that can be converted to true; otherwise, returns true.
