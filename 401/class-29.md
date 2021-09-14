# Routing

* The ``<Route>`` component is the main building block of React Router. Anywhere that you want to only render content based on the location’s pathname, you should use a ``<Route>`` element.
* React Router has been broken into three packages: ``react-router``, ``react-router-dom``, and ``react-router-native``.
* We are building a website (something that will be run in browsers), so we will install ``react-router-dom``.
* Type of Routing :
    1. The <BrowserRouter> should be used when you have a server that will handle dynamic requests (knows how to respond to any possible URI) 
    2. the <HashRouter> should be used for static websites (where the server can only respond to requests for files that it knows about).
*  router creates a **history** object, which it uses to keep track of the current location 1 and re-render the website whenever that changes and history object is mutable
* **Locations** represent where the app is now, where you want it to go, or even where it was.
* Router components only expect to receive a single child element. To work within this limitation, it is useful to create an ``<App>`` component that renders the rest of your application. 
* What does the <Route> render?
    1. component : A React component ``=======>`` When a route with a component prop matches, the route will return a new element whose type is the provided React component
    2. render : A function that returns a React element ``=======>``It will be called when the path matches
    3. children : A function that returns a React element``=======>`` this will always be rendered, regardless of whether the route’s path matches the current location.



# Term
* **props. children** does is that it is used to display whatever you include between the opening and closing tags when invoking a component.‏
* **Composition** pattern based on React's original component model where we build components from other components using explicit defined props or the implicit children prop


# Q
1. Do child components have direct access to props/state from the parent?
- we can see there is no way to pass props from a child component to a parent component. However, we can always pass around functions from the parent to child component. The child component can then make use of these functions. The function can then update the state in a parent component


2. When a component “wraps” another component, how does the child component’s output get rendered
- using props.children

3. Can a component, such as , which is a child also be used as a standalone component elsewhere in the application?
- Yes 

4. What trick can a parent use to share all props with it’s children
props
-  Cloning children with new props, You can use React.Children to iterate over the children, and then clone each element with new props (shallow merged) using React.cloneElement