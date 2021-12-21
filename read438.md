# Redux - Asynchronous Actions

## Review, Research, and Discussion 👍

How granular should your reducers be?

* It’s very easy to go full-warp with very specific events, dedicated for every change that occurs when a user is editing forms such as CHANGE_NAME, CHANGE_STREET, CHANGE_AGE, etc…

But it is not actually necessary if the logic behind the update is not different for all those fields. For those parts which require different handling in various reducers; dedicated action is the best solution. For others, sometimes a general action might be good enough.

Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched

It is a Pro more than a Con since we have to change multiple states in multiple components, the fact that all the reducers can listen when the action is dispatched can reduce a lot of work, each reducer can provide a different logic to the same dispatcher.

Name a strategy for preventing the above?
Make a reducer for each component that will be affected by the dispatcher, only effecting a specific amount of the state it self

-----------------------------------------------------------
--------------


### Document the following Vocabulary Terms 📑
|||
|-----|-----|
|store|A store is an immutable object tree in Redux. A store is a state container which holds the application's state. Redux can have only a single store in your application. Whenever a store is created in Redux, you need to specify the reducer|
|combined reducers|The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore . The resulting reducer calls every child reducer, and gathers their results into a single state object.|
|||





----------------------------------------------

## Preview 📙

1.Which 3 things had you heard about previously and now have better clarity on?

JSX,
context api,
class component

2.Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

AWS,
useEffect hook,
useReducer hook

3.What are you most excited about trying to implement or see how it works?

reducer hook & Redux

------------------------------


## Preparation Materials 📚



* Thunk middleware for Redux. It allows writing functions with logic inside that can interact with a Redux store's dispatch and getState methods.

* With a plain basic Redux store, you can only do simple synchronous updates by dispatching an action. Middleware extends the store's abilities, and lets you write async logic that interacts with the store.

* Thunks are the recommended middleware for basic Redux side effects logic, including complex synchronous logic that needs access to the store, and simple async logic like AJAX requests.


* By itself, a Redux store doesn't know anything about async logic. It only knows how to synchronously dispatch actions, update the state by calling the root reducer function, and notify the UI that something has changed. Any asynchronicity has to happen outside the store.

Earlier, we said that Redux reducers must never contain "side effects". A "side effect" is any change to state or behavior that can be seen outside of returning a value from a function. Some common kinds of side effects are things like:

Logging a value to the console
Saving a file
Setting an async timer
Making an AJAX HTTP request
Modifying some state that exists outside of a function, or mutating arguments to a function
Generating random numbers or unique random IDs (such as Math.random() or Date.now())


#### &copy; Dima Alabsi; 2021

