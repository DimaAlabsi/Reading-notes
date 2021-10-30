# Node Ecosystem, TDD, CI/CD


##  Array.map() method

* The Array.map() method allows you to iterate over an array and modify its elements using a callback function. The callback function will then be executed on each of the array's elements.

* The syntax for the map() method is as follows:

arr.map(function(element, index, array){  }, this);

---------------------

 ## Array.reduce()

 * The arr.reduce() method in JavaScript is used to reduce the array to a single value and executes a provided function for each value of the array (from left-to-right) and the return value of the function is stored in an accumulator.

* Syntax:

array.reduce( function(total, currentValue, currentIndex, arr), 
initialValue )


---------------

## superagent()

SuperAgent is light-weight progressive ajax API crafted for flexibility, readability, and a low learning curve after being frustrated with many of the existing request APIs. It also works with Node.js!

"
* Fetch Remote data ... superagent "returns a promise", so we can use `.then()`
superagent.get('http://demo8340031.mockable.io/stuff')
  .then( data => {
    console.log(data.body);
  })
  .catch(err => console.error(err));


* with async / await syntax :
'use strict';
const superagent = require('superagent');

let checkForWords = (words) => new Promise( (resolve,reject) => {

  let pauseTime = Math.ceil(Math.random()*1000);

  setTimeout( () => {
    if( words )  { resolve(`OK: ${words} / ${pauseTime}`) }
    else  { reject(`BAD: ${words} / ${pauseTime}`) }
  }, pauseTime)

});

// Using an old fashioned promise ...
checkForWords('coffee')
  .then( result => console.log(result) )
  .catch( console.error );


// Using an async function!
async function check(text) {
  try {
    let result = await checkForWords(text);
    console.log(result);
  } catch(e) { console.error(err); }

} " **quoted from  Code Fellows** 

---------------

* Async callbacks are functions that are specified as arguments when calling a function which will start executing code in the background. When the background code finishes running, it calls the callback function to let you know the work is done, or to let you know that something of interest has happened. Using callbacks is slightly old-fashioned now, but you'll still see them in use in a number of older-but-still-commonly-used APIs.

----------------------------

## Promises 
"
* A promise is commonly defined as a proxy for a value that will eventually become available.

Promises are one way to deal with asynchronous code, without getting stuck in callback hell.

Promises have been part of the language for years (standardized and introduced in ES2015), and have recently become more integrated, with async and await in ES2017.

Async functions use promises behind the scenes, so understanding how promises work is fundamental to understanding how async and await work.

* How promises work, in brief
Once a promise has been called, it will start in a pending state. This means that the calling function continues executing, while the promise is pending until it resolves, giving the calling function whatever data was being requested.

The created promise will eventually end in a resolved state, or in a rejected state, calling the respective callback functions (passed to then and catch) upon finishing. " [Read MORE!](https://nodejs.dev/learn/understanding-javascript-promises)

![promises](https://www.freecodecamp.org/news/content/images/2020/06/Ekran-Resmi-2020-06-06-12.21.27.png)





####  &copy; Dima Alabsi; 2021 
