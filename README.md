# lecture_2
## Table  of  Contents
> - 1) Scope
>
> - 2) Hoisting
>
> - 3) Recursion
>
> - 4) Closure

## What is SCOPE in JavaScript

>JavaScript has function scope: Each function creates a new scope.
>Variables defined inside a function are not accessible (visible) from outside the function.
>Variables declared with var, let and const are quite similar when declared inside a function.
>They all have Function Scope:

>Scope determines the accessibility (visibility) of variables.
>
>JavaScript has 3 types of scope:

> - 1)Block scope
>
> - 2)Function scope
>
> - 3)Global scope

## Block Scope

>Before ES6 (2015), JavaScript had only Global Scope and Function Scope.
>ES6 introduced two important new JavaScript keywords: let and const.
>These two keywords provide Block Scope in JavaScript.
>Variables declared inside a { } block cannot be accessed from outside the block:

![](https://pbs.twimg.com/card_img/1544656656906207233/Mjgb7Nqs?format=jpg&name=large)

## What is HOISTING in Javascript

>In JavaScript, a variable can be declared after it has been used.
>In other words; a variable can be used before it has been declared.

>Variables defined with let and const are hoisted to the top of the block, but not initialized.
>Meaning: The block of code is aware of the variable, but it cannot be used until it has been declared.
>Using a let variable before it is declared will result in a ReferenceError.
>The variable is in a "temporal dead zone" from the start of the block until it is declared:

>Var The scope of a variable declared with the keyword var is its current execution context. This is either the enclosing function or for variables declared outside any function, global.


>Hoisting: It is a concept that enables us to extract values of variables and functions even before initializing/assigning value without getting errors and this is happening due to the 1st phase (memory creation phase) of the Execution Context.


![](https://miro.medium.com/max/1200/1*3zcwke0wPy1t7n85o59HiQ.png)


## What is RECURSION in Javascript ?

>A recursive function is a function that calls itself.
>We can use it do divide a problem into a set of subproblems, each with a trivial solution.
>For instance, we can create a recursive function as follows:

![](/ima/photo_2023-03-16_14-44-13.jpg)

>In the code above, we have a simple recursive function that stops with i reaches 10.
>For each value of i , we log the value of i to the console.
>We should make sure that we have a base case to stop the function.
>If a function returns the result of running itself recursively, JavaScript doesn’t optimize that by replacing it with a loop.



## What is Closure in Javascript ?


>“A closure is the combination of a function bundled together (enclosed) with references to its surrounding state (the lexical 
>environment). In other words, a closure gives you access to an outer function’s scope from an inner function.”


>Closure is when a function is able to remember and access its lexical scope even when that function is executing outside its lexical scope.

>This is a closure because the nested function, returned when multiply5 is invoked, retains the reference to its state even after its parent function has finished executing.


![](https://res.cloudinary.com/practicaldev/image/fetch/s--1Xm29Qbp--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://user-images.githubusercontent.com/23126394/99179479-35df0600-2744-11eb-816f-c478399a246b.png)