![slice](https://capsule-render.vercel.app/api?type=slice&color=gradient&auto&height=200&text=State%20Redux&fontAlign=70&rotate=13&fontAlignY=25&desc=Done%20by%20Qasem%20Mohammad.&descAlign=70.&descAlignY=44)

# Redux - Additional Topics

## Redux Toolkit
* The official, opinionated, batteries-included toolset for efficient Redux development

### Redux Toolkit includes:
1. ***configureStore()*** function with simplified configuration options. It can automatically combine your slice reducers, adds whatever Redux middleware you supply, includes redux-thunk by default, and enables use of the Redux DevTools Extension.

2. **createReducer()** utility that lets you supply a lookup table of action types to case reducer functions, rather than writing switch statements.

3. **createAction()** utility that returns an action creator function for the given action type string. The function itself has toString() defined, so that it can be used in place of the type constant.

4. **createSlice()** function that accepts a set of reducer functions, a slice name, and an initial state value, and automatically generates a slice reducer with corresponding action creators and action types.

5. **createSelector** utility from the Reselect library, re-exported for ease of use.


### RTK Query
**RTK Query** is a powerful data fetching and caching tool. It is designed to simplify common cases for loading data in a web application, eliminating the need to hand-write data fetching & caching logic yourself.

# Trem 
* **middleware** Code usr to control req before send it to framework, existing between the framework receiving a request and the framework generating the response.

* **thunk** library in redux use to delay the action  

# Q
1. What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application? 
- thunk library in redux use to delay the action , and provide fir multiple reducer when commonly named action is dispatch 

2. When using a thunk/async action that dispatches the actual action, which do you export from your reducer?
- we export async function to handing api method then dispatch the action 