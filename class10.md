# Read: 10 - JS Debugging
![JSDebugging](https://firebearstudio.com/blog/wp-content/uploads/2015/10/Node.JS-Debugging-Tools.png)
To find the source of an error, it helps to know how scripts are processed.
The order in which statements are executed can be complex; some tasks
cannot complete until another statement or function has been run and that's knowen AS **ORDER OF EXECUTION**.

The JavaScript interpreter uses the concept of **execution contexts**.
There is one global execution context; plus, each function creates a new
new execution context. They correspond to variable scope. 


Every statement in a script lives in one of three
execution contexts:
* GLOBAL CONTEXT
Code that is in the script, but not in a function.
There is only one global context in any page.
* FUNCTION CONTEXT
Code that is being run within a function.
Each function has its own function context.
* EVAL CONTEXT (NOT SHOWN)
Text is executed like code in an internal function
called eva l {) (which is not covered in this book). 


Each time a script enters a new execution context, there are two phases of activity:
1. PREPARE
* The new scope is created
* Variables, functions, and arguments are created
* The value of the this keyword is determined

2. EXECUTE
* Now it can assign values to variables
* Reference functions and run their code
* Execute statements 

Understanding that these two phases happen helps
with understanding a concept called **hoisting.** You
may have seen that you can:
• Call functions before they have been declared
(if they were created using function declarations
- not function expressions, see p96)
• Assign a value to a variable that has not yet been
declared
This is because any variables and functions within
each execution context are created before they are
executed.

**Hoisting** is a process that moves all the declarations to the top of their scope. This is handled by the Javascript engine before running your code.


**Scope**
In the interpreter, each execution context has its own variables object. It holds the variables, functions, and parameters available within it. Each execution context can also access its parent's variables object.

**Errors**
If a JavaScript statement generates an error, then it throws an exception.
At that point, the interpreter stops and looks for exception-handling code. 

if you are anticipating that something in your code
may cause an error, you can use a set of statements
to **handle** the error (you meet them on p480).
This is important because if the error is not handled,
the script will just stop processing and the user will
not know why.

If you know your code might fail, use **try**, **catch**, and **finally**.
Each one is given its own code block.
```
try {
//II Try to execute this code
}
catch (exception) {
//II If there is an exception, run this code
}
finally {
//II This always gets executed
}
```


**Error objects** can help you find where your mistakes are and browsers have tools to help you read them. 
When there is an error, you can see all of this
information in the JavaScript **console** I Error console
of the browser. 

## A DEBUGGING WORKFLOW
Debugging is about deduction: eliminating potential causes of an error.
Try to narrow down where the problem might be, then look for clues. 

The JavaScript **console** will tell you when there is a problem with a script, where to look for the problem, and what kind of issue it seems to be.

You can also just type code into the console and it will show you a result. 

## BREAKPOINTS
You can pause the execution of a script on any line using breakpoints. Then you can check the values stored in variables at that point in time. 
![BP](https://d3of8ou1mslcoj.cloudfront.net/content/uploads/2012/05/javascript_breakpoints1.png)