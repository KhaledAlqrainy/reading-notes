# Component:

> Component is a portable set of functionality that encapsulates its implementation and exporting it as a higher-level interface, it has an obviously defined interface and conforms to a recommended behavior common to all components within an architecture.

## Component have three different views:

* **Object-oriented view:**

component is viewed as a set of one or more cooperating classes.

* **Conventional view :** 

It is viewed as a functional element or a module of a program that integrates the processing logic, the internal data structures that are required to implement the processing logic and an interface that enables the component to be invoked and data to be passed to it.

* **Process-related view :**

 The system is building the components from existing components maintained in a library.

## Advantages:

* **Ease of deployment** : As new compatible versions become available, it is easier to replace existing versions with no impact on the other components or the system as a whole.

* **Reduced cost**  The use of third-party components allows you to spread the cost of development and maintenance.

* **Ease of development** : Components implement well-known interfaces to provide defined functionality, allowing development without impacting other parts of the system.

* **Reusable** : The use of reusable components means that they can be used to spread the development and maintenance cost across several applications or systems.

* **Modification of technical complexity** : A component modifies the complexity through the use of a component container and its services.

* **Reliability** : The overall system reliability increases since the reliability of each individual component enhances the reliability of the whole system via reuse.

* **System maintenance and evolution** : Easy to change and update the implementation without affecting the rest of the system.

* **Independent** : Independency and flexible connectivity of components. Independent development of components by different group in parallel. Productivity for the software development and future software development.



# Props:

> it is a special keyword in React, which stands for properties and is being used for passing data from one component to another.

*  data with props are being passed in a uni-directional flow.

* props data is read-only, which means that data coming from the parent should not be changed by child components.


## How To Use Props In React:

* define an attribute and its data.

* pass the attribute to child component by using Props.

* render the Props Data
