# Props and State

## Understanding React `setState`
* **setState()** is the only legitimate way to update state after the initial state setup. 
* we’re passing an object to setState(). The object contains the part of the state we want to update which ``setState({ searchTerm: event.target.value })``
* **reconciliation** process is the way React updates the DOM, by making changes to the component based on the change in state. When the request to setState() is triggered
* **Object.assign()** is used to copy data from a source object to a target object
* benifit of ``setState()``
    1. Update to a component state should be done using setState()
    2. You can pass an object or a function to setState()
    3. Pass a function when you can to update state multiple times
    4. Do not depend on this.state immediately after calling setState() and make use of the updater function instead.


## Handling Events
* React events are named using camelCase, rather than lowercase.
* With JSX you pass a function as the event handler, rather than a string.
* cannot return false to prevent default behavior in React
* When using React, you generally don’t need to call addEventListener to add listeners to a DOM element after it is created. Instead, just provide a listener when the element is initially rendered.
* can Passing Arguments to Event Handlers with the React event (e)


## Forms
* **controlled component** making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input
* **Formik** is the world's most popular open source form library for React and React Native.

## State and Lifecycle

* You can convert a function component to a class in five steps:

    1. Create an ES6 class, with the same name, that extends React.Component.
    2. Add a single empty method to it called render().
    3. Move the body of the function into the render() method.
    4. Replace props with this.props in the render() body.
    5. Delete the remaining empty function declaration.

* Adding Local State to a Class We will move the date from props to state in three steps:
 1. Replace this.props.date with this.state.date in the render() method:
 2. Add a class constructor that assigns the initial this.state:
 3. Remove the date prop from the <calssName /> element:


## Components and Props
* Components let you split the UI into independent, reusable pieces, and think about each piece in isolation.
* define a component 
    1.  JavaScript function:
    2.  ES6 class 

* Composing Components

        function App() {

        return (

        <React.Fragment>

        <first Components/>

        <second Components" />

        </React.Fragment>

        );
        }


``ReactDOM.render(``

  ``<App />,``

  ``document.getElementById('root')``
``);``

*  we can split components into smaller components.
* All React components must act like pure functions with respect to their props.
* **puer function** not change their inputs, and always return the same result for the same inputs.


# Term
* **BDD** Behaviour-Driven Development is a collaborative approach to software development that bridges the communication gap between business and IT.
* **Acceptance Tests in software** test to  determination of whether the requirements of the normative project or legal contracts have been defined.
* **Mounting** is a process by which the operating system makes files and directories on a storage device (such as hard drive, CD-ROM, or network share) available for users to access via the computer's file system.
* **build** is the process of converting source code files into standalone software artifact(s) that can be run on a computer

# Q
1. Does a deployed React application require a server?
- You don't necessarily need a static server in order to run a Create React App project in production. It also works well when integrated into an existing server side app 

2. Why do we prefer to test a React application at the behavior rather than the unit level?
* easy to test the UI in front end
 
3. What does npm run build do?
- npm run build runs the script "build" and created a script which runs your application
- npm run build does nothing unless you specify what "build" does in your package.json file. It lets you perform any necessary building/prep tasks for your project, prior to it being used in another project.

4. Describe the actual composition / architecture of a React application
- Components written by different people should work well together. It is important to us that you can add functionality to a component without causing rippling changes throughout the codebase.
