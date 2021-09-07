# React and Forms

* **A Controlled Component is one that takes its current value through props and notifies changes through callbacks like onChange. A parent component "controls" it by handling the callback and managing its own state and passing the new values as props to the controlled component. You could also call this a "dumb component".**



 * *Controlled component is component that get the changed value from the callback function and uncontrolled component is component that have the one from the DOM. For example, When input value is changed,we can use onChange function in Controlled Component and also we can get the value using DOM like ref.*

 
 ![Controlled component](https://image.slidesharecdn.com/reacttutorialbasic-170330211625/95/basic-tutorial-of-react-for-programmers-80-638.jpg?cb=1490908827)

 * *An input is said to be “controlled” when React is responsible for maintaining and setting its state. The state is kept in sync with the input’s value, meaning that changing the input will update the state, and updating the state will change the input.*

 " ***React Forms vs. HTML Forms***
If you’ve worked with forms in plain HTML, a lot of this will probably seem familiar.

There’s a form tag, and labels for the inputs, same as you’d write in HTML.

Each label has an htmlFor prop that matches the id on its corresponding input. (That’s one difference: in HTML, the label attribute would be for. React uses htmlFor instead.)" quoted from [Dave Ceddia](https://daveceddia.com/react-forms/) ..

 [More information about Forms in React ..](https://www.youtube.com/watch?v=IkMND33x0qQ)

* *The input event is fired every time the value of the element changes. This is unlike the change event, which only fires when the value is committed, such as by pressing the enter key, selecting a value from a list of options, and the like.*

* ***A ternary operator allows you to assign one value to the variable if the condition is true, and another value if the condition is false. ... A ternary operator makes the assignment of a value to a variable easier to see, because it's contained on a single line instead of an if else block.***

   * Example of a ternary operator?
    + let num = 4, msg = "";
if (num === 4) {
  msg = "Correct!";
}
else {
  msg = "Incorrect!";
}


        + let x,y ;

    if (x===y){
        console.log("true")
        else{
            console.log(false);
        }
   
![](https://scotch-res.cloudinary.com/image/upload/w_auto,q_auto:good,f_auto/v1562952581/jqctyinrganjts991d3w.jpg)





 ####  &copy; Dima Alabsi; 2021 
