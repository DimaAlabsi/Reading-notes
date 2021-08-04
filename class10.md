 # Error Handling & Debugging

+  How to find the errors in your code:
    + HANDLING ERRORS
    +  COMMONPROBLEMS
    + THE CONSOLE & DEV TOOLS

"Execution context (EC) is defined as the environment in which the JavaScript code is executed. By environment, I mean the value of this, variables, objects, and functions JavaScript code has access to at a particular time." foma Rupesh Mishra..





![errors js](https://www.tutsmake.com/wp-content/uploads/2020/05/Types-of-Errors-In-JavaScript.jpeg)


HOW TO DEAL WITHERRORS  :
1: DEBUG THE SCRIPT TO FIX ERRORS
2: HANDLE ERRORS GRACEFULLY

![errors](https://www.javascripttutorial.net/wp-content/uploads/2019/12/javascript-try-catch-1-1.png)





" Type of errors in JavaScript
Jakub Włodarczyk
Jakub Włodarczyk

Mar 24, 2018·2 min read



Programming is a creative, demanding and rewarding activity. There are lots of cases when something can go wrong and we encounter errors in an application. Let’s take a look at types of errors in Javascript but first, let’s see how we can throw an example error:
try {
 throw Error('sample Error');
} catch (e) {
  console.log(e.message); sample Error
}
Without further ado, let’s take a look at the types:
SyntaxError — probably the most popular one while development. It tells us that the syntax of code is somehow invalid.

Example of syntax errors
![synatx error](https://miro.medium.com/max/423/1*bHYpkRC7C5HGKwaPslJ5IA.png)
TypeError — my number two as far as occurrence in development is concerned. Thrown when we have some value and it is not of a proper type.

Example of type errors
![type error](https://miro.medium.com/max/541/1*aadFSicd8Hr8nIer_5bZsg.png)
ReferenceError — thrown when we want to refer to some variable that doesn’t exist.

Example of reference errors
![refrenece error](https://miro.medium.com/max/518/1*bBC8TlPv5ouYsFxYxvKRzg.png)
RangeError —thrown when a value is not in an allowed range." this article quoted from Jakub Włodarczyk ,  
[its link ](https://medium.com/@wlodarczyk_j/type-of-errors-in-javascript-18458ba9d818)  .


 ####  &copy; Dima Alabsi; 2021 



