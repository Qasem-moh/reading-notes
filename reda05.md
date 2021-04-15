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
<!-- ![](https://i.ibb.co/sWFFsQs/6.png) -->