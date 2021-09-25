![slice](https://capsule-render.vercel.app/api?type=slice&color=gradient&auto&height=200&text=State%20Redux&fontAlign=70&rotate=13&fontAlignY=25&desc=Done%20by%20Qasem%20Mohammad.&descAlign=70.&descAlignY=44)

# Redux - Asynchronous Actions

* Redux Thunk is middleware that allows you to return functions, rather than just actions, within Redux. This allows for delayed actions, including working with promises. 
* Redux Thunk allows us to dispatch those actions asynchronously and resolve each promise that gets returned.

## what is the additional with thunk?
* With a plain basic Redux store, you can only do simple synchronous updates by dispatching an action. Middleware extends the store's abilities, and lets you write async logic that interacts with the store.


## work with thunk 
   1. install thunk ``npm install redux-thunk`` then import it 
   2. import ``applyMiddleware and createStore`` from redux
   3.  export stor and pass thunk as middleware ``export const store = createStore(countReducer, applyMiddleware(thunk));``
   4. Dispatch Function Instead of Object ==> Without redux-thunk, we are only allow to dispatch objects with a type property.


# Term 
* **store** is an immutable object tree in Redux. A store is a state container which holds the application's state. Redux can have only a single store in your application. Whenever a store is created in Redux, you need to specify the reducer.

* **combineReducers** helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore . The resulting reducer calls every child reducer, and gathers their results into a single state object.

# Q
1. How granular should your reducers be?
- The concept of a Reducer became popular in JavaScript with the rise of Redux as state management solution for React. ... Basically reducers are there to manage state in an application. For instance, if a user writes something in an HTML input field, the application has to manage this UI state (e.g. controlled components).

2. Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched
- Not always we need to fire all reducer in one action dispatch

3. Name a strategy for preventing the above
- thunk middleware in redux  that lets you write async logic that interacts with the store