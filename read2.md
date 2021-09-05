# State and Props


+ **The render happens first then the ‘componentDidMount’ at the component lifecycle events react..**

+ **Also those happen at the component lifecycle events react.. in the order** :

     + Constructor,
     + static getDerivedStateFromProps,
      + render, 
     + componentDidMount,
  + UNSAFE_componentWillMount 

![component lifecycle events react](https://miro.medium.com/max/834/1*yRAD50wbZEsTe6U4XNrMFA.png)

+ **componentDidMount loads anything using a network request or initialize the DOM..**

![component lifecycle events react](https://blog.logrocket.com/wp-content/uploads/2019/01/react-lifecycle-methods-diagram.png)


"What happens when state changes?
OK, why must we use setState( )? Why do we even need the state object itself? If you’re asking these questions, don't worry – you’ll understand state soon :) Let me answer.

A change in the state happens based on user-input, triggering an event, and so on. Also, React components (with state) are rendered based on the data in the state. State holds the initial information.

So when state changes, React gets informed and immediately re-renders the DOM – not the whole DOM, but only the component with the updated state. This is one of the reasons why React is fast.

And how does React get notified? You guessed it: with setState( ). The setState( ) method triggers the re-rendering process for the updated parts. React gets informed, knows which part(s) to change, and does it quickly without re-rendering the whole DOM.

In summary, there are 2 important points we need to pay attention to when using state:

State shouldn’t be modified directly – the setState( ) should be used
State affects the performance of your app, and therefore it shouldn’t be used unnecessarily
Can I use state in every component?
Another important question you might ask about state is where exactly we can use it. In the early days, state could only be used in class components, not in functional components.

That’s why functional components were also known as stateless components. However, after the introduction of React Hooks, state can now be used both in class and functional components.

If your project is not using React Hooks, then you can only use state in class components.

What are the differences between props and state?
Finally, let’s recap and see the main differences between props and state:

Components receive data from outside with props, whereas they can create and manage their own data with state
Props are used to pass data, whereas state is for managing data
Data from props is read-only, and cannot be modified by a component that is receiving it from outside
State data can be modified by its own component, but is private (cannot be accessed from outside)
Props can only be passed from parent component to child (unidirectional flow)
Modifying state should happen with the setState ( ) method " quoted from [**freeCodeCamp.org**](https://www.freecodecamp.org/news/react-js-for-beginners-props-state-explained/)

![prop & state](https://www.techdiagonal.com/wp-content/uploads/2019/09/react-props-blog-image-design-2.jpg)

+ The big difference between props and state:

*props you pass into a componont and the state is handled inside of componont and props are handled outside the componont
also when we change the state inside of our application it's going to render that section of the application but props we can't change them we  need to change them ouside the component*

+ *Props are like arguments when you create acomponont inside of react and we want to render it we're going to pass that*

![prop  state](https://i.stack.imgur.com/wqvF2.png)

[for more information eatvh this **video**](https://www.youtube.com/watch?v=IYvD9oBCuJI)

 #### &copy; Dima Alabsi; 2021 
