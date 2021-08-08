## **Node Ecosystem, TDD, CI/CD**

### ***Array.map()*** 

- It is an array method that is used to iterate over an array and that is used to returns a new array and elements of the original arrays are result of callback function.
  - return new array
  - need a return 
  - This method accepts two parameters 

### ***Array.reduce()***

- It is an array method that is executes a reducer function for each value of an array.
   - does not change the original array.
   - returns a single value which is the function's accumulated result.
   - need a return 
   

### ***superagent()***

- With normal Promise `.then()` syntax:

![Image](https://i.ibb.co/Zm278nV/s1.png)

- With `async / await` syntax

![image](https://i.ibb.co/zh11sQq/s2.png)

### ***promises*** 

- Promises, wrapping the asynchronous operation result, can be returned synchronously from a function, assigned to variables, or used as arguments. That’s the idea of promises: encapsulate the asynchronicity and allow function handling asynchronous operations to still look synchronous.
- A promise is an object that encapsulates the result of an asynchronous operation.
- Each promise has state, which can have one of the following values:

  - Pending
  - Fullfilled with a value
  - Rejected for a reason

### ***Are all callback functions considered to be Asynchronous? Why or Why Not?***
- No,Simply taking a callback doesn't make a function asynchronous. There are many examples of functions that take a function argument but are not asynchronous. For example there's `forEach` in Array. It iterates over each item and calls the function once per item.

