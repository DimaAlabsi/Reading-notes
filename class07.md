 # Object-Oriented Programming, HTML Tables 

 #### HTML tables :
 + Table represents information in a grid format.
 + < table> element is used to add tables to a web page.

 |||
 |------|------|
 |< table>|to create a table|
 |< tr>|At the end of the row you use a closing </ tr> tag|
 |< td>|Each cell of a table is represented using a < td> element|
 |< th>|sed just like the < td> element but its purpose is to represent the headin| forg either a column or a row.|
 |< thead>| The headings of the table should sit inside the < thead> element|
 |< tbody>|The body should sit inside the < tbody> elemen|
 |< tfoot>|The footer belongs inside the < tfoot> element|
 
![objectJS](https://fireship.io/courses/javascript/img/js-object-props.png)
" Functions allow you to group a set of related statements together that represent a single task.

Functions can take parameters (informatiorJ required to do their job) and may return a value.

An object is a series of variables and functions that represent something from the world around you. 

In an object, variables are known as properties of the object; functions are known as methods of the object.

Web browsers implement objects that represent both the browser window and the document loaded into the browser window.

JavaScript also has several built-in objects such as String, Number, Math, and Date. Their properties andmethods offer functionality that help you write scripts.


Arrays and objects can be used to create complex data sets (and both can contain the other)."   From the Duckett JS Book: Chapter 3: “Functions, Methods, and Objects” ( page : 144)..

#### Arrays are type of object
  + arrays hold set of key/value..
  + We can combine arrays and objects to create complex structure..

#### Three ways of Build-in OBJECTS:
  1- The Browser Object Model : contains objects that represent the current browser window or tab. 
  ![browser object model](https://ar.javascript.info/article/browser-environment/windowObjects.svg)

2- DOCUMENT OBJECT MODEL : The Document Object Model uses
objects to create a representation of
the current page.
![DOM](https://www.hebergementwebs.com/image/73/73552b2e32e69f617c91f449acfb5fbd.jpg/the-document-object-model-the-dom-and-its-role-for-the-web.jpg)

 3- The global JavaScript objects : represent things that the JavaScript language needs to create a model
of.

![THE GLOBAL OBJECT](https://i.ytimg.com/vi/YqGtvScabnk/maxresdefault.jpg)

 ![object](https://res.cloudinary.com/practicaldev/image/fetch/s--rJeH0yGE--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/t52ni02srb8688lh3eh8.png)

 + Create an intance of the DATE OBJECT :
 To specify the time and date..
 + Usind DATE OBJECT() ,Example :

   var today = new date();