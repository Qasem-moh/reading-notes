![slice](https://capsule-render.vercel.app/api?type=slice&color=gradient&auto&height=200&text=State%20Redux&fontAlign=70&rotate=13&fontAlignY=25&desc=Done%20by%20Qasem%20Mohammad.&descAlign=70.&descAlignY=44)

# combineReducers(reducers)

* As your app grows more complex, you'll want to split your reducing function into separate functions, each managing independent parts of the state.
* The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore.

* The resulting reducer calls every child reducer, and gathers their results into a single state object. The state produced by ``combineReducers()`` namespaces the states of each reducer under their keys as passed to ``combineReducers()``

* **Arguments ==>** reducers (Object): An object whose values correspond to different reducing functions that need to be combined into one.

* **Returns ==>**  (Function): A reducer that invokes every reducer inside the reducers object,

# Terms
* **immutable state** State cannot be modified, reducers must make copies of existing state to make updates.

* **time travel in redux** Redux DevTools records dispatched actions and the state of the Redux store at every point in time, which makes it possible to inspect the state and travel back in time to a previous application state without reloading the page or re-starting the app.

* **action creator** Instead of creating action objects inline in the places where you dispatch actions, can create functions generating them. You might write an action creator into a separate file, and import it into your component.

* **reducer** Functions that take current state and an action as arguments, and return a new state result, (state, action) => newState.

* **dispatch** A store holds the whole state tree of the application, the only way to change the state inside it is to dispatch an action on it.


# Q 
 1. Why choose Redux instead of the Context API for global state?
- Redux is the industry standard for managing the state of large applications. It is more optimized for larger projects because the context API re-renders more often.

 2. What is the purpose of a reducer?
- We need reducers to tell the application how to change state in response to an action. The action does not do anything except describe what happened and it is up to the reducer to respond to this.

 3. does an action contain?
- An action contains a action type and whatever payload you want it to have.

 4. Why do we need to copy the state in a reducer?
- The reducer needs to be a pure function without any side-effects. It should only take in an action and return the new state.