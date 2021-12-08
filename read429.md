 Component Lifecycle / useEffect()

## Review, Research, and Discussion 👍

How can we ensure that an effect hook runs only once?

by adding dependecies as an empty array , [] at the second argumenet

* Can useState() update more than one state variable at the same time?

Yes, by declare the state as an object{} 

* Is useState() synchronous?

It's Asynchronous 

-------------------------------------------------------------------------


### Document the following Vocabulary Terms 📑
|||
|-----|-----|
|State Hook|useState is a Hook that lets you add React state to function components|
|Component Lifecycle|Components are created (mounted on the DOM), grow by updating, and then die (unmount on DOM). This is referred to as a component lifecycle. There are different lifecycle methods that React provides at different phases of a component's life. ... At present, we know what lifecycle methods are and why they are important|






----------------------------------------------

## Preview 📙

1.Which 3 things had you heard about previously and now have better clarity on?

JSX,
events,
WRRC

2.Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

AWS,
useEffect hook,
useReducer hook

3.What are you most excited about trying to implement or see how it works?

AWS & Redux


----------------------------------------------

## Preparation Materials 📚

* **useReducer** is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.

* useReducer is one of the additional Hooks that shipped with React 16.8. An alternative to the useState Hook, it helps you manage complex state logic in React applications

* useReducer is used to store and update states, just like the useState Hook. It accepts a reducer function as its first parameter and the initial state as the second.

* useReducer returns an array that holds the current state value and a dispatch function, to which you can pass an action and later invoke. This is similar to the pattern Redux uses but with a few differences.

![useReducer Hook](https://dmitripavlutin.com/static/c47eb25d68bef042100d2b32083d7c0a/c1bf2/cover.png)


#### &copy; Dima Alabsi; 2021