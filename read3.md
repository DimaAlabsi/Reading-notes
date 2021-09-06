
# Passing Functions as Props


## lists and keys 




+ we  can loop through the array using the JavaScript map() function. We return an html element for each item. We include the entire  array inside an html element, and render it to the DOM


 "
 + **The map() method in JavaScript creates an array by calling a specific function on each element present in the parent array. It is a non-mutating method. Generally map() method is used to iterate over an array and calling function on every element of array.**

* Syntax:

array.map(function(currentValue, index, arr), thisValue)
Parameters: This method accepts two parameters as mentioned above and described below:

* function(currentValue, index, arr): It is required parameter and it runs on each element of array. It contains three parameters which are listed below:
* currentValue: It is required parameter and it holds the value of current element.
* index: It is optional parameter and it holds the index of current element.
* arr: It is optional parameter and it holds the array.
* thisValue: It is optional parameter and used to hold the value of passed to the function.

+ Return Value: It returns a new array and elements of arrays are result of callback function."
qouted from[geeksforgeeks](https://www.geeksforgeeks.org/javascript-array-map-method/)



![map methos](https://www.freecodecamp.org/news/content/images/size/w2000/2021/03/javascript-map-function.png)


### spread operator
*  spread syntax refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.

* it added to JavaScript in ES6 (ES2015), just like the rest parameters, which have the same syntax: three magic dots ….

##### the spread operator can do. :
* Copying an array
* Concatenating or combining arrays
* Using Math functions
* Using an array as arguments
* Adding an item to a list
* Adding to state in React
* Combining objects
* Converting NodeList to an array


    * an example of using the spread operator to combine two arrays:
   const arr1 = [1,2,3]
   const arr2 = [4,5,6]
   const arr3 = [...arr1, ...arr2] //arr3 ==> [1,2,3,4,5,6]
   -----
 *  an example of using the spread operator to add a new item to an array:
  const arr1 = ['a', 'b'];
const arr2 = ['c', 'd', 'e'];

arr.push(...arr2);

console.log(arr); // ['a', 'b', 'c', 'd', 'e']

-------
 * an example of using the spread operator to combine two objects :
 
 let person = {
    firstName: 'John',
    lastName: 'Doe',
    age: 25,
    ssn: '123-456-2356'
};


let job = {
    jobTitle: 'JavaScript Developer',
    location: 'USA'
};

let employee = {
    ...person,
    ...job
};

console.log(employee);


* Output:

{
    firstName: 'John',
    lastName: 'Doe',
    age: 25,
    ssn: '123-456-2356',
    jobTitle: 'JavaScript Developer',
    location: 'USA'
}ts into one.



* You can pass state values to a child component as a prop, but you can also pass functions directly to the child component like this:

<ChildComponent
    // The child component will access using actionName
    actionName={this.actual_action_name}
/>
         *  actionName is the name of the props that can be accessed by the child component. 


* You can  pass a method from a parent component into a child component:

    *   A parent component defines a function

     * The function is passed as a prop to a child component

    * The child component then invokes the prop

     *         The parent function is then called, usually changing something

     *    Then the parent component is re-rendered along with its children

![parent and child component](https://i.stack.imgur.com/CCruc.jpg)


#### How does the child component invoke a method that was passed to it from a parent component?
"
React.forwardRef
React.forwardRef creates a React component that forwards the ref attribute, which it receives, to another component below in the tree. So, in simple words forwardRef creates such a component which receives a ref attribute from its parent component and forwards it to the components down in the hierarchy.
Arguments and return type: React calls this function with two arguments one is props and the other is ref. This returns a react node something like this." quoted from[Nugen I.T. Services](https://medium.com/@nugen/react-hooks-calling-child-component-function-from-parent-component-4ea249d00740)




![compontes](https://miro.medium.com/max/875/1*2FvzWlnqEG11zbUX98uMQQ.jpeg)

 #### &copy; Dima Alabsi; 2021 



