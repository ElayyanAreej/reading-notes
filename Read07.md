## Operators
* Assignment operators

simple assignment operator is **equal (=)**, which assigns the value of its right operand to its left operand. That is, ``` x = y ``` assigns the value of y to x.
* Comparison operators

A comparison operator compares its operands and returns a logical value based on whether the comparison is true.

| Operator    | Name                  |
| ----------- | -----------           |
|    ==       | Equal                 |  
|    !=       | Not equal             |  
|    ===      | Strict equality       |  
|    !==      | Non-equality          |
|     <       | Less than	            |
|     >       | Greater than          |
|     >=      | Greater than or equal |
|     <=      | Less than or equal    |

👉
*Note* 	
Strict equality returns true if the operands are equal and of the same type.


* Arithmetic operators

An arithmetic operator takes numerical values (either literals or variables) as their operands and returns a single numerical value.

| Operator    | Name           |
| ----------- | -----------    |
|      +      | Addition       |  
|      -      | Subtraction    |
|      *      | Multiplication |
|      /      | Division       |
|      %      | Remainder      |  
|     ++      | Increment      |
|     --      | Decrement      |
|     **      | Exponentiation |

* Bitwise operators

A bitwise operator treats their operands as a set of 32 bits (zeros and ones), rather than as decimal, hexadecimal, or octal numbers.

* Logical operators

Logical operators are typically used with **Boolean** (logical) values; when they are, they return a Boolean value. 


 *Logical AND* **&&** returns true if both operands are true,otherwise returns false.

 *Logical OR* **||** returns true if either operand is true; if both are false, returns false.

 *Logical NOT* **!** returns false if its single operand that can be converted to true; otherwise, returns true.

* String operators

In addition to the comparison operators, which can be used on string values, the concatenation operator (+) concatenates two string values together, returning another string that is the union of the two operand strings.

* Conditional (ternary) operator
 ```
condition ? val1 : val2
 ```
 If condition is true, the operator has the value of val1. Otherwise it has the value of val2. You can use the conditional operator anywhere you would use a standard operator.   
* Comma operator

 The comma operator (,) evaluates both of its operands and returns the value of the last operand.used inside a for loop, to allow multiple variables to be updated each time through the loop.

* Unary operators

A unary operation is an operation with only one operand.
delete

* Relational operators

A relational operator compares its operands and returns a Boolean value based on whether the comparison is true.


## Control flow
The control flow is the order in which the computer executes statements in a script.
![cf](https://blog.jscrambler.com/content/images/2017/03/control-flow-flattening01.jpg)
Code is run in order from the first line in the file to the last line, unless the computer runs across the (extremely frequent) structures that change the control flow, such as conditionals and loops. 

## JavaScript Functions

A JavaScript function is a block of code designed to perform a particular task.

A JavaScript function is executed when "something" invokes it (calls it).

**Syntax**

```
function name(parameter1, parameter2, parameter3) {
  // code to be executed
}
```
Function **parameters** are listed inside the *parentheses ()* in the function definition.

Function **arguments** are the values received by the function when it is *invoked*.


👉👉
*Notes* 

-Inside the function, the arguments (the parameters) behave as **local variables**.

-When JavaScript reaches a **return statement**, the function will stop executing.

-If the function was invoked from a statement, JavaScript will "return" to execute the code after the invoking statement.