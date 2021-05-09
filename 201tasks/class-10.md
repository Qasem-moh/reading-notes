# Error Handling and Debugging

_It can be difficult to learn and master JavaScript without making mistakes, but it is best to learn how to troubleshoot errors using developer tools as well. When you write JavaScript for the first time, it will not be easy to avoid errors, and errors can be found through the browser, where it tells you about the errors that occurred._

## Tools For Developer

- THE CONSOLE & DEV TOOLS
  Tools built into the browser
  that help you hunt for errors.
- COMMON PROBLEMS
  Common sources of errors,
  and how to solve them.
  HANDLING ERRORS
  How code can deal with
  potential errors gra cefully.

## ORDER OF EXECUTION

To find the source of an error, it helps to know how scripts are processed.
The order in which statements are executed can be complex; some tasks
cannot complete until another statement or function has been run:

## EXECUT.ION CONTEXTS

The JavaScript interpreter uses the concept of execution contexts.
There is one global execution context; plus, each function creates a new
new execution context. They correspond to variable scope.

# EXECUTION CONTEXT& HOISTING

Each time a script enters a new execution context, there are two phases of activity:

1: **PREPARE**

- The new scope is created
- Variables, functions, and arguments are created
- The value of the this keyword is determined

2: **EXECUTE**

- Now it can assign values to variabl es
- Reference functions and run their code
- Execute statements

## UNDERSTANDING SCOPE

In the interpreter, each execution context has its own variables object.
It holds the variables, functions, and parameters available within it.
Each execution context can also access its parent's variables object.

Functions in JavaScript are said to have lexical scope.
They are linked to the object they were defined within.
So, for each execution context, the scope is the
current execution context's variables object, plus the
variables object for each parent execution context.Imagine that each function is a nesting doll.
The children can ask the parents for information in
their variables. But the parents cannot get variables
from their children. Each child will get the same
answer from the same parent.

# UNDERSTANDING ERRORS

If a JavaScript statement generates an error, then it throws an exception.
At that point, the interpreter stops and looks for exception-handling code.

If you are anticipating that something in your code may cause an error, you can use a set of statements to handle the error.This is important because if the error is not handled, the script will just stop processing and the user will not know why. So exception-handling code should inform users when there is a problem.

## ERROR OBJECTS

Error objects can help you find where your mistakes are
and browsers have tools to help you read them.
![ERROR OBJECTS](https://i.ibb.co/ngVK1WR/image.png)

## HOW TO DEAL WITH ERRORS

Now that you know what an error is and how the browser treats them,
there are two things you can do with the errors.

1: DEBUG THE SCRIPT TO FIX ERRORSIf you come across an error while writing a script
(or when someone reports a bug), you will need to debug the code, track down the source of the error, and fix it. You will find that the developer tools available in
every major modern browser will help you with this task. In this chapter, you will learn about the developer tools in Chrome and Firefox. (The tools in Chrome is identical to those in Opera.) IE and Safari also have their own tools.

2: HANDLE ERRORS GRACEFULLY

You can handle errors gracefully using try, catch, throw, and finally statements.Sometimes, an error may occur in the script for a reason beyond your control. For example, you might request data from a third party, and their server
may not respond. In such cases, it is particularly important to write error-handling code. In the latter part of the chapter, you will learn how to
gracefully check whether something will work, and offer an alternative option if it fails.


