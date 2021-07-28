# The Mock

The mock looks like the following image :


![](https://reactjs.org/static/1071fbcc9eed01fddc115b41e193ec11/d4770/thinking-in-react-mock.png)

> now the first thing we want to do is to break the UI into components and make thim insied boxses,  **single responsibility principle** its a way that a component should ideally only do one thing. 
If it ends up growing, it should be decomposed into smaller subcomponents.

**we have five components in our app :**

* **FilterableProductTable** (orange): contains the entirety of the example

* **SearchBar (blue)** : receives all user input

* **ProductTable (green)**: displays and filters the data collection based on user input

* **ProductCategoryRow (turquoise)**: displays a heading for each category

* **ProductRow (red)** : displays a row for each product

when we identified the components in our mock we have to arrange them into a hierarchy, Components that appear within another component in the mock should appear as a child in the hierarchy:


> The Second thing we have to Build A Static Version in React

* in this step we will implement our app: 

we want to build components that reuse other components and pass data using props.

> the thirs step is to Identify The Minimal Representation Of UI State

 DRY: Don’t Repeat Yourself. we will Figure out the absolute minimal representation of the state your application needs and compute everything else we need on-demand.

  We have pieces of data :

  * The original list of products

* The search text the user has entered
* The value of the checkbox
* The filtered list of products

> the fourth step is to Identify Where our State Should Live

For each piece of state in your application we have to do the following:

* Identify every component that renders something based on that state.

* Find a common owner component (a single component above all the components that need the state in the hierarchy).

* Either the common owner or another component higher up in the hierarchy should own the state.

* If we can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

> the final step is to Add Inverse Data Flow.

 **FilterableProductTable** will pass callbacks to SearchBar that will fire whenever the state should be updated. We can use the onChange event on the inputs to be notified of it. The callbacks passed by FilterableProductTable will call setState(), and the app will be updated.