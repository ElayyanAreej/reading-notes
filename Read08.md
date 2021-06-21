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

# Loops and iteration
 Quick and easy way to do something repeatedly.



![pic](https://i.ytimg.com/vi/eSYeHlwDCNA/maxresdefault.jpg)

There are many different kinds of loops, but they all essentially do the same thing: they repeat an action some number of times.

### for statement 
Repeats until a specified condition evaluates to false.
```
for ([initialExpression]; [conditionExpression]; [incrementExpression])
  statement
  ```

### do...while statement
Repeats until a specified condition evaluates to false.

```
do
  statement
while (condition);
```
👉👉
*Notes*

-statement is always executed once before the condition is checked.

-To execute multiple statements, use a block statement (``` { ... } ```) to group those statements.

### while statement

Executes its statements as long as a specified condition evaluates to true. 
```
while (condition)
  statement
  ```
  #### **labeled statement**
  A label provides a statement with an identifier that lets you refer to it elsewhere in your program. 
  ```
  label :
   statement
   ```

  #### **break statement**
Use the break statement to terminate a loop, switch, or in conjunction with a labeled statement.
  ![](https://cdn.programiz.com/sites/tutorial2program/files/javascript-break-statement.png)

#### **continue statement**
![](https://cdn.programiz.com/sites/tutorial2program/files/java-continue.png)
When you use continue without a label, it terminates the current iteration of the innermost enclosing while, do-while, or for statement and continues execution of the loop with the next iteration.

When you use continue with a label, it applies to the looping statement identified with that label.