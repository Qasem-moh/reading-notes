# Component Composition

## The Component Lifecycle

1. **Mounting**
* first method that runs is the constructor method
* render method which returns JSX
* ``componentDidMount`` inside of it we ca do any asynchronous calls to databases or directly manipulate the DOM 


2. **Updating** 
* call ``getDerivedStateFromProps``
* ``getDerivedStateFromProps`` you can compare old props/state with the new set of props/state. You can determine if your component should re-render or not by returning true or false
* ``getSnapshotBeforeUpdate``  It allows the engineer to capture some information about the DOM before it's changed

3. **Unmounting**
* this phase is that last stage of the component lifecycle. When you remove a component from the DOM, React runs ``componentWillUnmount`` right before it gets removed. You should use this method to clean up any open connections such as WebSockets or intervals.

## Higher-Order Components(HOC)
* A higher-order component is a function that takes a component and returns a new component.
* **setState()** : method The only way you should change state

## props.children
* **stateless function** is just a plain javascript function which takes props as an argument and returns a react element, and there is no ``this`` keyword 
* we use props.children on components that represent '‘'generic boxes' 

## composition & inheritance
* recommend  use composition instead of inheritance to reuse code between components.

## Term
* **component props**  a keyword in React stands for properties, can be any information that needs to be passed to another component.

* **component state** : The state is an instance of React Component Class can be defined as an object of a set of observable properties that control the behavior of the component.

* **application state**: is interface between data and the representation of this data with UI elements on the front-end. 

# Q
1. Can a parent component access the state of a child component? Yes but not directly
2. What can be passed along in a prop variable? any data you want to passed.
3. How can a child component “know” the state of another component? By sending and getting the data from the parent