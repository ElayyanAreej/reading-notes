# Read: 06 - JS Object Literals; The DOM
> Understanding The Problem Domain Is The Hardest Part Of Programming.
By John Sonmez

## Why ? 
![icon](https://cdn2.iconfinder.com/data/icons/coding-9/256/coding_piece_puzzle_html_design-512.png)

Try to put together a jigsaw puzzle that didn’t have any picture on it !!! The reason why puzzles like this one are so hard, is because you **can’t** really **see what you are trying to build** very clearly.

The **same** thing happens when **writing code**.  Writing code is a lot like putting together a jigsaw puzzle.  We put together code with the purpose of building components that we have taken out of the “bigger picture” of the problem domain.


You could spent days trying to implement a feature but if you go back and talk to a product owner and hash out completely how something should work and why it should work in a particular way, only to go back to your desk and crank out the code in a matter of hours.

***It is very difficult to solve a problem before you know the question.***

## What can you do about it?
If understanding the problem domain is the hardest part of programming and you want to make programming easier, you can do one of two things:

1. Make the problem domain easier.
2. Get better at understanding the problem domain.


***You can often make the problem domain easier by cutting out cases and narrowing your focus to a particular part of the problem.***

---
## WHAT IS AN OBJECT? 
Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object, variables and functions take on new names. 
* If a variable is part of an object, it is called a
**property**. Properties tell us about the object.
* If a function is part of an object, it is called a **method**. Methods represent tasks that are associated with the object. 

👉
*Notes* 
-An object cannot have two keys with the same name.This is because keys are used to access their corresponding values.
-The value of a property can be a string, number,Boolean, array, or even another object. The value of a
method is always a function.

### Creating An Object

```
let objectName = {
    //properties
    //method{}
};
```

### Accessing An Object
```
let variable=objectName.property/method Name();
```

## Document Object Model
![DOM](https://upload.wikimedia.org/wikipedia/commons/thumb/5/5a/DOM-model.svg/1200px-DOM-model.svg.png)
THE DOM TREE IS A MODEL OF A WEB PAGE

As a browser loads a web page, it creates a model of that page.
The model is called a DOM tree, and it is stored in the browsers' memory.
It consists of four main types of nodes. 


Each node is an object with methods and properties.
Scripts access and update this DOM tree (not the source HTML file).
Any changes made to the DOM tree are reflected in the browser. 

### Accessing and updating the DOM tree involves two steps:
1. Locate the node that represents the element you want to work with.

2. Use its text content, child elements, and attributes. 