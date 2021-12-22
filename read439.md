# Redux - Additional Topics

## Review, Research, and Discussion 👍

What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?
The most 'redux-like' way of handling the pre-loading of data would be to fire off the asynchronous action in the lifecycle method (probably componentWillMount ) of a Higher Order Component that wraps your app

When using a thunk/async action that dispatches the actual action, which do you export from your reducer?


To dispatch async actions into our store, we have to apply the thunk middleware by writing: const store = createStore(joke, applyMiddleware(thunk)); to apply the middleware. Then in App , we call dispatch with the function returned from the fetchJoke passed inside

-----------------------------------------------------------
--------------


### Document the following Vocabulary Terms 📑
|||
|-----|-----|
|middleware| type of computer software that provides services to software applications beyond those available from the operating system|
|thunk|middleware for Redux. It allows writing functions with logic inside that can interact with a Redux store's dispatch and getState methods.|



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

Thunk & Redux

------------------------------


## Preparation Materials 📚

* Redux Toolkit
The official, opinionated, batteries-included toolset for efficient Redux development



Simple

Opinionated

Powerful

Effective  [Redux Toolkit](https://redux-toolkit.js.org/)


* State is the heart of each application and there is no quicker way to create buggy, unmanageable applications than by producing an inconsistent state or state that is out-of-sync with local variables that linger around. 

![](https://mobx.js.org/assets/getting-started-assets/overview.png)


* Hookstate

The simple but incredibly fast and flexible state management that is based on React state hook [Know MORE](https://hookstate.js.org/)

#### &copy; Dima Alabsi; 2021