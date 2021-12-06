# useState() Hook

## Review, Research, and Discussion 👍

**How does React differ from vanilla JS/HTML/CSS**

* Plain JS apps usually start with the initial UI created on the server (as HTML), whereas React apps start with a blank HTML page, and dynamically create the initial state in JavaScript. React requires you to break your UI into components, but plain JS apps can be structured in any way you see fit.

* What makes React such a desirable library to learn is that it doesn't replace HTML. It takes advantage of HTML's popularity and strength as the most popular programming language, by letting you use a very similar syntax to HTML to build interfaces and add dynamic features to it using JavaScript.

***What is the primary difference between a function component and a class component?***

*  Functional component is just a plain JavaScript function that accepts props as an argument and returns a React element. A class component requires you to extend from React. Component and create a render function which returns a React element. There is no render method used in functional component

![](https://miro.medium.com/max/1400/1*6-bN_FxEMfRTHZSouF8DLg.png)




--------------------------------------------------------------------------


### Document the following Vocabulary Terms 📑
|||
|-----|-----|
|Functional Components|Functional components are basic JavaScript functions. These are typically arrow functions but can also be created with the regular function keyword. Sometimes referred to as “dumb” or “stateless” components as they simply accept data and display them in some form; that is they are mainly responsible for rendering UI.|
|Children / Child Components|There is one prop that gets special treatment unlike all the others. That,Children allow you to pass components as data to other components, just like any other prop you use. The special thing about children is that React provides support through its ReactElement API and JSX. XML children translate perfectly to React children!|

----------------------------------------------

## Preview 📙

1.Which 3 things had you heard about previously and now have better clarity on?

JSX,
events,
WRRC

2.Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

AWS,
REACT.js,
UDP

3.What are you most excited about trying to implement or see how it works?

Hooks  & react.js

----------------------------------------------

## Preparation Materials 📚

* ***Hooks*** are functions that let you “hook into” React state and lifecycle features from function components. Hooks don't work inside classes — they let you use React without classes. ... You can also create your own Hooks to reuse stateful behavior between different components.

* Hooks are a new addition in React 16.8. They let you use state and other React features without writing a class.


* Hooks apply the React philosophy (explicit data flow and composition) inside a component, rather than just between the components.

* Hook is a react function that lets you use state and react features from a function based component. Hooks let you use the functions instead of switching between HOCs, Classes, and functions. As Hooks are regular Javascript functions, thus you can use the built-in Hooks and create your own custom one.

* Hooks can cover all use cases for classes while providing more flexibility in extracting, testing, and reusing code. However one reason that you should still go for Class components over the function components with hooks until Suspense is out for data fetching.


**Hooks example** 

![hooks example](https://miro.medium.com/max/2000/1*irVQowoE01OYqAsuGzHycg.png)

 #### &copy; Dima Alabsi; 2021