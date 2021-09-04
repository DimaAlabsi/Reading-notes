# Introduction to React and ComponentsWhat is a Component?


 

"A component is a modular, portable, replaceable, and reusable set of well-defined functionality that encapsulates its implementation and exporting it as a higher-level interface.

A component is a software object, intended to interact with other components, encapsulating certain functionality or a set of functionalities. It has an obviously defined interface and conforms to a recommended behavior common to all components within an architecture.

A software component can be defined as a unit of composition with a contractually specified interface and explicit context dependencies only. That is, a software component can be deployed independently and is subject to composition by third parties." qouted from  [tutorialspoint](https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm)

**The charactistics of a component** :
+ Independent 
+ Encapsulated 
+ Extensible 
+ Not context specific
+ Replaceable 
+ Reusability 


 ***The advantages of using component based architecture*** :
  + Independent 
  + System maintenance and evolution
 + Modification of technical complexity
 + Reliability 
 + Reusable 
 + Ease of development
+  Reduced cost
 + Ease of deployment
 





 " **React** is a component-based library which divides the UI into little reusable pieces. In some cases, those components need to communicate (send data to each other) and the way to pass data between components is by using props.
“Props” is a special keyword in React, which stands for properties and is being used for passing data from one component to another.
But the important part here is that data with props are being passed in a uni-directional flow. (one way from parent to child). " quoted from [INTEXT](https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0)


### Using Props in React :
+ *define an attribute and its value(data)**
+ *pass it to child component(s) by using Props* 
+ *render the Props Data*

![component](https://www.codevoila.com/cvuploads/images/201607/reactjs_component_lifecycle_status.png)

 #### **data with props are being passed in a uni-directional flow. (one way from parent to child)**


![props](https://miro.medium.com/max/1838/1*bsS8ETUQqgBpAoT2D6tjmw.png)



 **React is a declarative, efficient, and flexible JavaScript library for building user interfaces. It lets you compose complex UIs from small and isolated pieces of code called “components”.**