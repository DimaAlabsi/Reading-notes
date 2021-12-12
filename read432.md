#  Context API - Behaviors

## Review, Research, and Discussion 👍



When you have multiple contexts, what component type should you use (class/function) and why?


In class components, the render method will be called, whenever the state of the components changes. On the other hand, the Functional components render the UI based on the props. Class Components should be preferred whenever we have the requirement with the state of the component


What are some good use cases for using the Context API for global state?

* Context is primarily used when some data needs to be accessible by many components at different nesting levels.


* How can you best test context?

The best way to test Context is to make our tests unaware of its existence and avoiding mocks. We want to test our components in the same way that developers would use them (behavioral testing) and mimic the way they would run in our applications (integration testing).


-------------------------------------------------------------------------


### Document the following Vocabulary Terms 📑
|||
|-----|-----|
|context| React's context allows you to share information to any component, by storing it in a central place and allowing access to any component that requests it (usually you are only able to pass data from parent to child via props)|
|useContext()|useContext” hook is used to create common data that can be accessed throughout the component hierarchy without passing the props down manually to each level. Context defined will be available to all the child components without involving “props”.|
|static context|This rule applies when the static contextType property of a React component is not properly specified. The contextType property is used to consume a context created with React.|




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