# Hooks API

### Hooks are a new addition in React 16.8. They let you use state and other React features without writing a class.
* Hooks let us organize the logic inside a component into reusable isolated units to prevent faced **Huge components** that are hard to refactor and test.or **Duplicated logic** between different components and lifecycle methods.or **Complex patterns** like render props and higher-order components.

*  the usage of Hook is to enable you to add state into function instead of converting the function to class by using Hook inside function 


* Hook use in the top level of the React functions
* Hooks return to react function only ; can't use in JS function 
* ``Hook state`` is method to declare state in react function 

* **useEffect** : use to replace a lifecycle method , and  when we have side effects that need to happen along with each change
* **useState** :  use to access state and you can call useState as many times as you want, like with setState
* **useContext** :how to consume a provider using a hook, Accepts a context object



## Five Important Rules for Hooks
1. Never call Hooks from inside a loop, condition or nested function
2. Hooks should sit at the top-level of your component
3. Only call Hooks from React functional components
4. Never call a Hook from a regular function
5. Hooks can call other Hooks

# Term 
* **React Composition** is a development pattern based on React's original component model where we build components from other components using explicit defined props or the implicit children prop

*  **Children** allow you to pass components as data to other components, just like any other prop you use. The special thing about children is that React provides support through its ReactElement API and JSX. XML children translate perfectly to React children

* **Hash Routing** Using the anchor part of the URL to simulate different content.

* **Link Routing** Provides declarative, accessible navigation around your application.

# Q
1. Why do we not need more .html pages in a multi-page React app?  
- Because we use SP concept to build react App; so we render all component in the same page after load server 

2. If we wanted a component to show up on every page, where would we put it and why?
- Inside the ``<BrowserRouter />`` and outside ``<Route />``  

3. What does props.children contain?
- every thing between the opening and closing tag 