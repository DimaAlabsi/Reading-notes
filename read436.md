# API Integration
## Review, Research, and Discussion 👍

What are the advantages of storing tokens in “Cookies” vs “Local Storage”

t's just less convenient for the attacker because they can't read the content of the token although they rarely have to. It might also be more advantageous for the attacker to attack using victim's browser (by just sending that HTTP Request) rather than using the attacker's machine.


Explain 3rd party cookies.

Third-party cookies are cookies that are set by a website other than the one you are currently on. For example, you can have a "Like" button on your website which will store a cookie on a visitor's computer, that cookie can later be accessed by Facebook to identify visitors and see which websites they visited.


How do pixel tags work?

tracking pixel (also called 1x1 pixel or pixel tag) is a graphic with dimensions of 1x1 pixels that is loaded when a user visits a webpage or opens an email. ... The tracking pixel URL is the memory location on the server. When the user visits a website, the image with the tag is loaded from this server

-----------------------------------------------------------
--------------


### Document the following Vocabulary Terms 📑
|||
|-----|-----|
|cookies|Cookies are data, stored in small text files, on your computer. When a web server has sent a web page to a browser, the connection is shut down, and the server forgets everything about the user|
|authorization| the process of giving someone permission to do or have something|
|access control|a security technique that regulates who or what can view or use resources in a computing environment. |
|conditional rendering|term to describe the ability to render different user interface (UI) markup if a condition is true or false. In React, it allows us to render different elements or components based on a condition|




----------------------------------------------

## Preview 📙

1.Which 3 things had you heard about previously and now have better clarity on?

JSX,
context api,
class component

2.Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

AWS,
useEffect hook,
useReducer hook

3.What are you most excited about trying to implement or see how it works?

reducer hook & Redux

------------------------------


## Preparation Materials 📚

* Redux is a predictable state container for JavaScript apps.

* Redux provides a solid, stable, and mature solution to managing state in your React application


* Redux is an open-source JavaScript library for managing and centralizing application state. It is most commonly used with libraries such as React or Angular for building user interfaces. Similar to (and inspired by) Facebook's Flux architecture, it was created by Dan Abramov and Andrew Clar

* Redux is most useful when in cases when:
     * You have large amounts of application state that are needed in many places in the app.
     * The app state is updated frequently.
     * The logic to update that state may be complex.
     * The app has a medium or large-sized codebase, and might be worked on by many people

* Reducers
Just a quick refresher on what reducer is before we go into testing and code. Redux documentation is still great, in fact it covers unit tests really well you don’t even have to read this post. To summarize it, the reducer is a pure function that takes the previous state and an action, and returns the next state.

[Redux Docs](https://redux.js.org/)

#### &copy; Dima Alabsi; 2021
