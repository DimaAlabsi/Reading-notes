#  Context API

## Review, Research, and Discussion 👍


Describe use cases useState() vs useReducer() ?


* useState is the way if we need an internal state and don't need to implement more complex logic such as lifecycle methods

* seReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks


Why do custom hooks need the use prefix?

* custom Hook doesn't need to have a specific signature. ... Its name should always start with use so that you can tell at a glance that the rules of Hooks apply to it

What do custom hooks usually do?

* Custom hooks allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks

Using any list of custom hooks, research and name one that you think will be useful in your applications

* Instead, always use Hooks at the top level of your React function, before any early returns. By following this rule, you ensure that Hooks are called in the same order each time a component renders. That's what allows React to correctly preserve the state of Hooks between multiple useState and useEffect calls.

Describe how a hook that fetches API data might work?


Now we need to fetch the data from the API with the useEffect hook. import React, { useState, useEffect } from 'react'; function App() { 
    const [data, setData] = useState([]); 
    useEffect(() => { // here goes the data fetching }); return ( < ul> {data. map(item => ( < li key={item.id}> < a href={item. url}>{item.

-------------------------------------------------------------------------


### Document the following Vocabulary Terms 📑
|||
|-----|-----|
|reducer|useReducer is one of the additional Hooks that shipped with React 16.8. An alternative to the useState Hook, it helps you manage complex state logic in React application|






----------------------------------------------

## Preview 📙

1.Which 3 things had you heard about previously and now have better clarity on?

JSX,
events,
class component

2.Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

AWS,
useEffect hook,
useReducer hook

3.What are you most excited about trying to implement or see how it works?

reducer hook & Redux


----------------------------------------------

## Preparation Materials 📚

***Context provides a way to pass data through the component tree without having to pass props down manually at every level***

* Context provides a way to share values like these between components without having to explicitly pass a prop through every level of the tree.

* Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult.

* Creates a Context object. When React renders a component that subscribes to this Context object it will read the current context value from the closest matching Provider above it in the tree.

* The defaultValue argument is only used when a component does not have a matching Provider above it in the tree. This default value can be helpful for testing components in isolation without wrapping them. Note: passing undefined as a Provider value does not cause consuming components to use defaultValue.

![context](https://res.cloudinary.com/practicaldev/image/fetch/s--YxjWiLSY--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://www.carlrippon.com/static/0d1f722d0fe4c2bc4c3d71595dbe67dd/ca682/prop-drilling-v-context.png)


![contextt](https://dmitripavlutin.com/90649ae4bdf379c482ad24e0dd220bc4/react-context-3.svg)


[READ MORE](https://medium.com/swlh/snackbars-in-react-an-exercise-in-hooks-and-context-299b43fd2a2b)

#### &copy; Dima Alabsi; 2021