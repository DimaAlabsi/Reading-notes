# Component Based UI

## Review, Research, and Discussion 👍

**Name 5 Javascript UI Frameworks (other than React)**

Ember.js


AngularJS

Vue.js

Sencha

Webix

**What’s the difference between a framework and a library**

Framework
 
In a framework, all the control flow is already there and there are many predefined white spots that we should fill out with our code. A framework is normally more complex. It defines a skeleton where the application defines its own features to fill out the skeleton. In this way, your code will be called by the framework appropriately. The benefit is that developers do not need to worry about if a design is good or not, but just about implementing domain-specific functions. The framework will provide you with hooks and call-backs so that you build on it; it will then call your plugged-in code whenever it wishes, a phenomenon called Inversion of Control.
 
A framework can contain libraries. A framework will usually include many libraries to make your work easier.
 
Library
 
A library performs specific, well-defined operations. A library is just a collection of class definitions. The reason is it simply code reuse, in other words, gets the code that has already been written by other developers. The classes and methods normally define specific operations in a domain-specific area. For example, there are some libraries of mathematics that can let developers just call the function without redoing the implementation of how an algorithm works. A library will usually focus on a single piece of functionality that you access using an API. You call a library function, it executes some code and then the control is returned to your code.


--------------------------------------------------------------------------


### Document the following Vocabulary Terms 📑
|||
|-----|-----|
|Rendering|The most important procedure that a programmer has to manage in frontend development. In React, the render() method is the only required method in a class component, and is responsible for describing the |
|Templates|ets of ready-to-use parts of code built using React technology for the development of dynamic user interfaces.|
|State|a plain JavaScript object used by React to represent an information about the component's current situation|
----------------------------------------------

## Preview 📙

1.Which 3 things had you heard about previously and now have better clarity on?

Socket,
events,
WRRC

2.Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

AWS,
Tree data structure,
UDP

3.What are you most excited about trying to implement or see how it works?

AWS & react.js


----------------------------------------------

## Preparation Materials 📚

* JSX : it is a syntax extension to JavaScript. We recommend using it with React to describe what the UI should look like. JSX may remind you of a template language, but it comes with the full power of JavaScript.

* Example :

**const element = < h1>Hello, world!</ h1>;**

* React embraces the fact that rendering logic is inherently coupled with other UI logic: how events are handled, how the state changes over time, and how the data is prepared for display

* Unlike browser DOM elements, React elements are plain objects, and are cheap to create. React DOM takes care of updating the DOM to match the React elements.

* React is a JavaScript library for building user interfaces. This guide targets React v15 to v16. 
[READ MORE](https://devhints.io/react)


***REACT JS example***

![react.js](https://miro.medium.com/max/1400/1*KKL94ILBNpmH1RKLgsCRiw.png)
 #### &copy; Dima Alabsi; 2021