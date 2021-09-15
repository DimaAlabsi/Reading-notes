# In memory storage

+ **When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.**

+ ***The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.***



***(LIFO) is one of these inventory valuation methods. It assumes that the last items placed in invent***

  +  an example of a call stack and the functions that would need to be invoked to generate that call stack :

  function firstFunction(){
  throw new Error('Stack Trace Error');
}

function secondFunction(){
  firstFunction();
}

function thirdFunction(){
  secondFunction();
}

thirdFunction(); 

![JS](https://i.ytimg.com/vi/2ZH_1d8TYVg/maxresdefault.jpg)
---------------------------

+ A **stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.**


### Types of ERRORS

+ **Reference errors**

" This is as simple as when you try to use a variable that is not yet declared you get this type os errors. 

This is also a common thing when using const and let, they are hoisted like var and function but there is a time between the hoisting and being declared so when you try to access them a reference error occurs, the fact that this happens to let and const is called Temporal Dead Zone (TDZ).

+ **syntax error** : this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

+ **Range errors** : Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.

+ **Type errors** :Like the name indicates, this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.

***The breakpoint can also be achieved by putting a debugger statement in your code in the line you want to break.***

***You can run the debugger by pressing F5 or pressing the green play button.*** " [Read MORE](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

![error](https://javascript.info/article/try-catch/try-catch-flow.svg)


















####  &copy; Dima Alabsi; 2021 
