# Redux - Combined Reducers

## Review, Research, and Discussion 👍

Why choose Redux instead of the Context API for global state?

 Redux uses React’s Context API behind the scenes! Redux is more than just a simple wrapper around Context though – 

What is the purpose of a reducer?

A reducer is a function that determines changes to an application’s state. It uses the action it receives to determine this change

What does an action contain?

Redux actions are JavaScript objects that contain two properties: type and payload. These actions are "dispatched," or used as arguments by the Redux store's dispatch API method. A typical Redux action looks as follows: { type: 'ADD_POST', payload: { id: 1, title: 'Redux Tutorial 2019' } }

Why do we need to copy the state in a reducer?

If the new state is different, the reducer must create new object, and making a copy is a way to describe the unchanged par

-----------------------------------------------------------
--------------


### Document the following Vocabulary Terms 📑
|||
|-----|-----|
|immutable state|its value cannot be changed once it's created. A mutable state allows us to modify already created data structures and change them whichever way we want|
|time travel in redux|Time travel is the ability to move back and forth among the previous states of an application and view the results in real time.|
|action creator|is a function that literally creates an action object. In Redux, action creators simply return an action object and pass the argument value if necessary. These action creators are passed to the dispatch function as the result value, and the dispatch is executed|
|reducer| pure function that takes an action and the previous state of the application and returns the new state. The action describes what happened and it is the reducer's job to return the new state based on that action|
|dispatch|dispatch is a function of the Redux store. You call store. dispatch to dispatch an action. This is the only way to trigger a state change. With React Redux, your components never access the store directly - connect does it for you|




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



* Redux is an open-source JavaScript library for managing and centralizing application state. It is most commonly used with libraries such as React or Angular for building user interfaces. Similar to (and inspired by) Facebook's Flux architecture, it was created by Dan Abramov and Andrew Clar

* Redux is most useful when in cases when:
     * You have large amounts of application state that are needed in many places in the app.
     * The app state is updated frequently.
     * The logic to update that state may be complex.
     * The app has a medium or large-sized codebase, and might be worked on by many people

* Reducers
Just a quick refresher on what reducer is before we go into testing and code. Redux documentation is still great, in fact it covers unit tests really well you don’t even have to read this post. To summarize it, the reducer is a pure function that takes the previous state and an action, and returns the next state.

* Multiple Reducers with Redux Reducers 👍

It turns out that Redux lets us combine multiple reducers into one that can be passed into createStore by using a helper function named combineReducers . The way we combine reducers is simple, we create one file per reducer in the reducers directory. We also create a file called index. js inside the reducers directory

* The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore.

* The resulting reducer calls every child reducer, and gathers their results into a single state object. The state produced by combineReducers() namespaces the states of each reducer under their keys as passed to combineReducers()

[Redux Docs: Using Combined Reducers](https://redux.js.org/usage/structuring-reducers/using-combinereducers/)

#### &copy; Dima Alabsi; 2021
