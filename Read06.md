# Dynamic web pages with JavaScript
## JavaScript
 is a lightweight, interpreted, or just-in-time compiled programming language with first-class functions.
 JavaScript allows you to implement complex features on web pages more than just sit there and display static information.

#### It is the third layer of the layer cake of standard web technologies !
 😅 🍰

![pic](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/What_is_JavaScript/cake.png)

1. ***HTML*** is the markup language that we use to structure 
2. ***CSS*** is a language of style rules that we use to apply styling to our HTML content.
3. ***JavaScript*** is a scripting language that enables you to create dynamically updating content. 

👉 
*Note* Do not ~~~confuse~~~ JavaScript with the Java programming language. Both "Java" and "JavaScript" are trademarks or registered trademarks of Oracle in the U.S. and other countries. However, the two programming languages have very ***different syntax, semantic, and use***.



### So what can it really do?
* Store useful values inside variables. 
* Operations on pieces of text (known as "strings" in programming). 
* Running code in response to certain events occurring on a web page.
* And much more!

### How do you add JavaScript to your page?
1. **Internal JavaScript**
By adding script element to the HTML page, Scripts can be placed in the body, or in the head section of an HTML page, or in both. You can place any number of scripts in an HTML document.

👉
 *Note* Placing scripts **at the bottom of the body** element **improves the display speed**, because script interpretation slows down the display.

```
<script>

  // JavaScript goes here

</script>
```

2. **External JavaScript**
By create a **new file** in the same directory as your sample HTML file. Call it script.js — make sure it has that **.js** filename extension, as that's how it is recognized as JavaScript.
Then we linked the file to HTML page.
```
<script src="script.js" defer></script>
```
👉 
*Note* JavaScript is **case sensitive**, and very fussy, so you need to enter the syntax exactly as shown, otherwise it may not work.

*** Thinking like a programmer
One of the hardest things to learn in programming is not the syntax you need to learn.***

![thinking](https://base.imgix.net/files/base/ebm/industryweek/image/2020/04/problem_solving.5e962254a8281.png?auto=format&fit=max&w=1200.png)

### ***syntax***
- ** Comments **
```
//A single line comment.
```
```
/*
A multi-line comment.
........ 
/*
```

- ** variables **

with the keyword **let (or var) or const** followed by a name for your variable.
const keyword to define a variable that cannot be reassigned,and the let keyword to define a variable with restricted scope.
```
var variableName = num or string or boolean value;
```
👉👉*Notes* 

-Remember that JavaScript identifiers (names) must begin with:
 - A letter (A-Z or a-z)
 - A dollar sign ($)
 - Or an underscore (_)
 -In What_is_JavaScript
 
-The equal sign (=) is an "assignment" operator, not an "equal to" operator.

-Strings are written inside double or single quotes. Numbers are written without quotes.

-You can declare many variables in one statement, just Start the statement with var and separate the variables by comma.
 Example:
```
var person = "John Doe", carName = "Volvo", price = 200;
```

-A variable declared without a value will have the value undefined.



- **Functions**
Functions are reusable blocks of code that you can write once and run again and again, saving the need to keep repeating code all the time. 

Defined a function by using the **keyword function**, followed by a name, with parentheses put after it. After that we put two curly braces. Inside the curly braces goes all the code that we want to run whenever we call the function.
```
function checkGuess() {
  alert('I am a placeholder');
}
```

- **Operators**
allow us to perform tests, do math, join strings together, and other such things.


| Operator    | Name           |
| ----------- | -----------    |
|      +      | Addition       |  
|      -      | Subtraction    |
|      *      | Multiplication |
|      /      | Division       |



👉👉
*Notes*

 -You can also use the + operator to join text strings together (in programming, this is called concatenation).
```
name += ' says hello!';
```
 -If you put a number in quotes, the rest of the numbers will be treated as strings, and concatenated.

*Note* You can also use the + operator to join text strings together (in programming, this is called concatenation).
```
name += ' says hello!';
```


| Operator    | Name                  |
| ----------- | -----------           |
|    ===      | Strict equality       |  
|    !==      | Non-equality          |
|     <       | Less than	            |
|     >       | Greater than          |

- **Conditionals**
 A conditional code block allows you to run code selectively, depending on whether a certain condition is true or not. conditional block starts with the **keyword if**, then some parentheses, then some curly braces. Inside the parentheses we include a test. If the test returns true, we run the code inside the curly braces. If not, we don't, and move on to the next bit of code.
 ```
 if(test){
   // True case code;
 }
 ```
 ![h](https://craftofcoding.files.wordpress.com/2020/04/controlstr_if1.jpg)

- ** Loops**
Allow you to keep running a piece of code over and over again, until a certain condition is met.

```
for ( starting value ; condition ; incrementor) { 
  console.log(i) }

  ```
![loopimg](https://www.tenouk.com/clabworksheet/labworksheet7_files/cforloopflowchart001.png)

## Input and Output in JS
To get input from the user we use **getElementById**.
Example:
```
 var fname = document.getElementById('first_name').value;
 ```

**JavaScript Output**
* Writing into an HTML element, using **innerHTML**.
* Writing into the HTML output using **document.write()**.
* Writing into an alert box, using **window.alert()**.
* Writing into the browser console, using **console.log()**.

## Types of error
Generally speaking, when you do something wrong in code, there are two main types of error that you'll come across:
* **Syntax errors**: These are **spelling** errors in your code that actually cause the program not to run at all.

* **Logic errors**: These are errors where the syntax is actually correct but the code is not what you intended it to be, meaning that program runs successfully but gives **incorrect results**. 


