# Logical Operators
***
_A logical operator is a symbol or word used to connect two or more expressions such that the value of the compound expression produced depends only on that of the original expressions and on the meaning of the operator.[1] Common logical operators include AND, OR, and NOT._
***
_Within most languages, expressions that yield Boolean data type values are divided into two groups. One group uses the relational operators within their expressions and the other group uses logical operators within their expressions._

_The logical operators are often used to help create a test expression that controls program flow. This type of expression is also known as a Boolean expression because they create a Boolean answer or value when evaluated. There are three common logical operators that give a Boolean value by manipulating other Boolean operand(s). Operator symbols and/or names vary with different programming languages:_
![operator](https://i.ibb.co/gSYK0Z3/3.png)
***
**A common way to show logical relationships is in truth tables.**
![](https://i.ibb.co/p0PsjDL/4.png)
## && (AND)
#### The AND operator is represented with two ampersands &&:
result = a && b;
![](https://i.ibb.co/0sMFpC9/11.png)
**An example with if:**
![](https://i.ibb.co/84sYVcR/12.png)

**Just as with OR, any value is allowed as an operand of AND:**

![](https://i.ibb.co/GWwn22R/13.png)
**AND “&&” finds the first falsy value**
**result = value1 && value2 && value3;**
_The AND && operator does the following:
* Evaluates operands from left to right.
* For each operand, converts it to a boolean. If the result is false, stops and returns the original value of that operand.
* If all operands have been evaluated (i.e. all were truthy), returns the last operand.
In other words, AND returns the first falsy value or the last value if none were found.
The rules above are similar to OR. The difference is that AND returns the first falsy value while OR returns the first truthy one.
Examples:_
![](https://i.ibb.co/x1t16rF/14.png)

_We can also pass several values in a row. See how the first falsy one is returned:_
![](https://i.ibb.co/bQ2nGPj/15.png)



*****
***
_In classical programming, the logical OR is meant to manipulate boolean values only. If any of its arguments are true, it returns true, otherwise it returns false.
In JavaScript, the operator is a little bit trickier and more powerful. But first, let’s see what happens with boolean values.
There are four possible logical combinations:_
![](https://i.ibb.co/FBWLs34/8.png)
***


_As we can see, the result is always true except for the case when both operands are false.
If an operand is not a boolean, it’s converted to a boolean for the evaluation.
For instance, the number 1 is treated as true, the number 0 as false:_
![](https://i.ibb.co/pbs8RPv/5.png)

***
**Most of the time, OR || is used in an if statement to test if any of the given conditions is true.**
![](https://i.ibb.co/Fzt7cLh/7.png)
#### We can pass more conditions:
![](https://i.ibb.co/rdSgLLy/66.png)
_OR "||" finds the first truthy value
The logic described above is somewhat classical. Now, let’s bring in the “extra” features of JavaScript.The extended algorithm works as follows. Given multiple OR’ed values:
result = value1 || value2 || value3;
The OR || operator does the following:
Evaluates operands from left to right.
For each operand, converts it to boolean. If the result is true, stops and returns the original value of that operand.
If all operands have been evaluated (i.e. all were false), returns the last operand.
A value is returned in its original form, without the conversion.
In other words, a chain of OR || returns the first truthy value or the last one if no truthy value is found.
For instance:_
![](https://i.ibb.co/GHn0yG9/9.png)
*** 
![](https://i.ibb.co/sWFFsQs/6.png)
**! (NOT)**
The boolean NOT operator is represented with an exclamation sign !.

The syntax is pretty simple:
![](https://i.ibb.co/d0t4FGc/16.png)
_The operator accepts a single argument and does the following:

1. Converts the operand to boolean type: true/false.
2. Returns the inverse value.
For instance:_
![](https://i.ibb.co/kx0yc3q/17.png)
### A double NOT !! is sometimes used for converting a value to boolean type:
![](https://i.ibb.co/DW90Nkh/18.png)
_That is, the first NOT converts the value to boolean and returns the inverse, and the second NOT inverses it again. In the end, we have a plain value-to-boolean conversion.
There’s a little more verbose way to do the same thing – a built-in Boolean function:_
![](https://i.ibb.co/bv00T63/19.png)
***

![](https://i.ibb.co/z5pQPbX/20.png)
**Equality operators: == and !=**
![]()
## Syntax
expression == expression
expression != expressio

Sometimes it is required to compare the value of one variable with other. The comparison operators take simple values (numbers or string) as arguments and evaluate either true or false. Here is a list of comparison operators.

![](https://i.ibb.co/f40TLD0/21.png)
**JavaScript Equal (==) operator**
Pictorial presentation of Equal (==) operato
![](https://www.w3resource.com/w3r_images/js-equal-operator.png)
2   ==  2   // true
2   ==  3   // false
2   == '2'  // true
"4" ==  4   // true
***
_Example of JavaScript Equal (==) operator
The following function first evaluates if the condition (num == 15) evaluates to true. If it does, it returns the statement between the curly braces (“Equal”). If it doesn’t, it returns the next return statement outside them (“Not equal”).
JavaScript Code:_
![](https://i.ibb.co/khsw2rh/22.png)
**JavaScript Strict Equal (===) operator**
![](https://www.w3resource.com/w3r_images/js-strict-equal-operator.png)
5 ===  5   // true
5 === '5'  // false
Example of JavaScript Strict equal (===) operator

The following function first evaluates if the condition (num === 15) evaluates to true. If it does, it returns the statement between the curly braces ("Equal"). If it doesn’t, it returns the next return statement outside them ("Not equal").

JavaScript Code:
![](https://i.ibb.co/8xBxttB/23.png)
JavaScript Not equal (!=) operator
Pictorial presentation of Not equal(!=) operator
![](https://www.w3resource.com/w3r_images/js-not-equal-to-operator.png)
3 !=  4     // true
3 != "3"    // false
3 != '3'    // false
3 != true   // false
0 != false  // false
<br>
****
![](https://i.ibb.co/KqRqsS0/24.png)
***
JavaScript Strict not equal (!==) operator
Pictorial presentation of Strict not equal(!==) operator
![](https://www.w3resource.com/w3r_images/js-strict-not-equal-operator.png)
2 !==  2   // false
2 !== '2'  // true
3 !==  2   // true
***
Example of JavaScript Strict Not equal (!==) operator

The following function first evaluates if the condition (num !== 15) evaluates to true considering both value and value type. If it does, it returns the statement between the curly braces ("Not equal"). If it doesn’t, it returns the next return statement outside them ("Equal").
JavaScript Code:
![](https://i.ibb.co/g4d9MV6/25.png)
***



**Thanks**