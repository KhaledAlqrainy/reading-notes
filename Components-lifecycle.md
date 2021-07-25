# Components lifecycle

> there are three Phases in the components life cycle:

* **Mounting** : when creating inctanes and inserted in the DOM.

* **Updating** : when change or update the component.

* **Unmounting** : when remove the component.

### There is alot of code we can use such as:

* componentDidMount() :  If you need to load anything using a network request or initialize the DOM, it should go here.

* shouldComponentUpdate() :  This is in order to optimize performance,  If shouldComponentUpdate() returns false, then UNSAFE_componentWillUpdate(), render(), and componentDidUpdate() will not be invoked.

* componentWillUnmount() : This method allows you to clean up the DOM and netwrok requests/ subscriptions.

* 
