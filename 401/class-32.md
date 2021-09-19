# Custom Hooks
* Custom Hooks are JavaScript functions whose names are prefixed with the word  we adding the word use to the beginning, it lets us know that this function follows the rules of Hooks.
* Unlike a React component, a custom Hook doesn’t need to have a specific signature. We can decide what it takes as arguments, and what, if anything, it should return.

## React Hooks with Async-Await
* we go to make our custom hook which search for result instead of use promises or 'Async-await : to make our code cleaner and single liner on final usage. It must be not redundant
* We cannot use 'async' keyword with 'useEffect' callback method. It will result in race conditions.

## useReducer
* **useReducer** is one of the additional Hooks that shipped with React 16.8. An alternative to the useState Hook, it helps you manage complex state logic in React 

* useReducer is **used to** store and update states, just like the useState Hook. It **accepts** a reducer function as its first parameter and the initial state as the second

* useReducer **returns** an array that holds the current state value and a dispatch function, to which you can pass an action and later invoke

# Terms 
* **state hook** the state add by the feature of hook function like ``useState``
* **Effect Hook** lets you perform side effects in function components, and replace lifecycle methods
* **useReducer** is a hook I use sometimes to manage the state of the application, It acts as an alternate hook to the useState hook to manage complex state in your application.

# Q
1. What does a component’s lifecycle refer to?
- Everything you see in a React application is a component or part of a component. In React, components are designed to follow the natural cycle of life. They are born (creation), grow (updating), and finally die (deletion). This is called the component lifecycle


2. Why do you sometimes need to “wrap” functions in useCallback when called from within useEffect
- in ``useEffect`` no need to re-create function component  render 


3. Why are functional components preferred over class components?
- functional components  easer to read and presentational 


4. What is wrong with the following code?
- we can't use ``UseEffect` inside loop 
