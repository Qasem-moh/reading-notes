# State and Props

Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

**render**

What is the very first thing to happen in the lifecycle of React?

**Mounting**

Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates

1- constructor

2- render

3-React Updates

4-componentDidMount

5-componentWillUnmount

## What are component lifecycle events?

React lets you define components as classes or functions. The methods that you are able to use on these are called lifecycle events. These methods can be called during the lifecycle of a component, and they allow you to update the UI and application states.

![lifecycle](https://miro.medium.com/max/2800/0*0saPKFiTUk6W3FYp)


**Mounting, Updating, and Unmounting are the three phases of the component lifecycle.**

**Mounting**

When an instance of a component is being created and inserted into the DOM it occurs during the mounting phase. Constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount all occur in this order during mounting.

****

**Updating**

Anytime a component is updated or state changes then it is rerendered. These lifecycle events happen during updating in this order.
static getDerivedStateFromProps, shouldComponentUpdate, render,
getSnapshotBeforeUpdate, componentDidUpdate, UNSAFE_componentWillUpdate, UNSAFE_componentWillReceiveProps
***

**Unmounting**

The final phase of the lifecycle if called when a component is being removed from the DOM. componentWillUnmount is the only lifecycle event during this phase.

**constructor()**

The constructor for a React component is called before it is mounted.If the component is a subclass you should call super(props), or the props will be undefined. constructors can be used to assign state using this.state or to bind event handle methods to an instance. Let’s take a look at some example code.