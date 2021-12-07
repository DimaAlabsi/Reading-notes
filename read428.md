# Component Lifecycle / useEffect()

## Review, Research, and Discussion 👍
Why do we not need more .html pages in a multi-page React app?

* A React app consists of a single HTML file index.html. The views are coded in JSX format as components.


If we wanted a component to show up on every page, where would we put it and why?
Outside the < BrowserRouter/>
Inside the < BrowserRouter />, outside a < Route />
Inside a <Route />

***Inside the < BrowserRouter />, outside a < Route />***


What does routing do with the components that were rendered when a new route is requested

it becomes with a new componetnt & delete the old ones


What does props.children contain?


props. children does is that it is used to display whatever you include between the opening and closing tags when invoking a component. example: 
 component contains an < img> that is receiving some props and then it is displaying {props. children} .

How do useState() and this.setState() differ?


*setState() does not immediately mutate this. state but creates a pending state transition. Accessing this. state after calling this method can potentially return the existing value.




--------------------------------------------------------------------------


### Document the following Vocabulary Terms 📑
|||
|-----|-----|
|State Hook|A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components.|
|Mounting and Un-Mounting|The mount command mounts a storage device or filesystem, making it accessible and attaching it to an existing directory structure. The umount command "unmounts" a mounted filesystem, informing the system to complete any pending read or write operations, and safely detaching it.|

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

AWS & react.js


----------------------------------------------

## Preparation Materials 📚


**The Effect Hook**

* The function passed to useEffect will run after the render is committed to the screen. Think of effects as an escape hatch from React’s purely functional world into the imperative world.

By default, effects run after every completed render, but you can choose to fire them only when certain values have changed.

* A functional React component uses props and/or state to calculate the output. If the functional component makes calculations that don't target the output value, then these calculations are named side-effects.

Examples of side-effects are fetch requests, manipulating DOM directly, using timer functions like setTimeout(), and more.

The component rendering and side-effect logic are independent. It would be a mistake to perform side-effects directly in the body of the component, which is primarily used to compute the output.


* ***useEffect() hook accepts 2 arguments:***

useEffect(callback[, dependencies]);

* callback is the function containing the side-effect logic. callback is executed right after changes were being pushed to DOM.

* dependencies is an optional array of dependencies. useEffect() executes callback only if the dependencies have changed between renderings.

 #### &copy; Dima Alabsi; 2021