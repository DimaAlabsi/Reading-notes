

# FUNCTIONAL PROGRAMMING
***Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data***



![ functional programming](https://cdn.guru99.com/images/1/080118_0618_WhatisFunct1.png)



![pure functions](https://www.modernescpp.com/images/blog/Functional/PureFunctions/CharakteristikPureFunctionsEng.png)


* **pure functions** :

  + It returns the same result if given the same arguments (it is also referred as deterministic)
  + It does not cause any observable side effects



![pure fun](https://cdn-media-1.freecodecamp.org/images/0*a_yub2gTwY-1eK8j.png)



+ Benefits of pure functions
My favorite benefits of pure functions are:

    + They’re easier to reason about
    + They’re easier to combine
    +  They’re easier to test
     + They’re easier to debug
     +    They’re easier to parallelize


------------------

+ **immutability** :
Unchanging over time or unable to be changed.

+ If a function consistently yields the same result for the same input, it is referentially transparent.

   + pure functions + immutable data = referential transparency

   + A **module** is a software component or part of a program that contains one or more routines. One or more independently developed modules make up a program. An enterprise-level software application may contain several different modules, and each module serves unique and separate business operations.

   + The require() method is used to load and cache JavaScript modules. So, if you want to load a local, relative JavaScript module into a Node. js application, you can simply use the require() method.


"   **The static import statement is used to import read only live bindings which are exported by another module.**

Imported modules are in strict mode whether you declare them as such or not. The import statement cannot be used in embedded scripts unless such script has a type="module". Bindings imported are called live bindings because they are updated by the module that exported the binding.

There is also a function-like dynamic import(), which does not require scripts of type="module".

Backward compatibility can be ensured using attribute nomodule on the < script> tag." [Read MORE](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/import)

+ Exporting module features
The first thing you do to get access to module features is export them. This is done using the export statement.

+ The easiest way to use it is to place it in front of any items you want exported out of the module, 
   #### &copy; Dima Alabsi; 2021 
