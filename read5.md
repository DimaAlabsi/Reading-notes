#  Putting it all together


" **Before creating an app, you should create a rough wireframe of it. A wireframe is nothing but a visual  representation of the skeletal framework of your app. This will give you a clear view of what your app is going to look like.**

 * #### Basic layout of the page
 
 * #### Breaking it into components
 Once your wireframe is ready, you can start breaking it into individual components. Now, this can be tricky for beginners. What can be considered as a component?

***A component is anything that has its standalone meaning in the layout.***

***For example, a calculator has a screen and many buttons. The screen is a component as it has its separate use of just displaying the calculations. An individual button is also a component. And finally, the whole calculator can be considered as a root component as it integrates the screen and the button components together.***

So, after breaking my layout into components, I come up with the structure below.

*  #### create a component hierarchy —

***Start from the root component (App). It will be the root node of the tree.
Find it’s direct children components (Intro and Skills)***

*  #### Make a tree and represent App as the root node and Intro and Skills its children.

Now, repeat the same process with other component nodes. Find direct children of the components from Figure "
 [javascript-essentials](https://medium.com/javascript-essentials/the-best-approach-to-design-react-component-hierarchy-978bb152dbb2)



![create a component hierarchy ](https://beginnersbook.com/wp-content/uploads/2015/06/awt_hierarchy.png)


---------------

 * ***The single-responsibility principle (SRP) is a computer-programming principle that states that every module, class or function in a computer program should have responsibility over a single part of that program's functionality, and it should encapsulate that part.***


* "  **The easiest way is to build a version that takes your data model and renders the UI but has no interactivity. To build a static version of your app that renders your data model, you’ll want to build components that reuse other components and pass data using props.**"[Read more about build a ‘static’ version of your application?](https://stackoverflow.com/questions/49428116/building-static-version-of-react-application)





     *  #### What are the three questions you can ask to determine if something is state?

        *  What is the difference between state and props                        
        
        * Why is setState giving me the wrong value?

        * How do I update state with values that depend on the current state?
Identify every component that renders something based on that state.


" ***Find a common owner component (a single component above all the components that need the state in the hierarchy).***

Either the common owner or another component higher up in the hierarchy should own the state.
If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component." [Read more](https://reactjs.org/docs/thinking-in-react.html)



![state](https://res.cloudinary.com/practicaldev/image/fetch/s--czFD1ROI--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://www.tutsmake.com/wp-content/uploads/2020/05/javascript-promises-states.jpeg)
















####  &copy; Dima Alabsi; 2021 
