# Controlled Components

> the form in HTML hase elemnents and it can be updated based on the user but in React there is muiltple state and can be updated only wit setState().

>  An input form element whose value is controlled by React in this way is called a “controlled component”.

> With a controlled component, the input’s value is always driven by the React state.

**Some of tags used in React form :**

* **The textarea Tag** : uses a value attribute.

* **The select Tag** : uses a value attribute on the root select tag. This is more convenient in a controlled component because you only need to update it in one place. 

* **The file input Tag** : it is an uncontrolled component in React. It is discussed together with other uncontrolled components later in the documentation.

### Handling Multiple Inputs

> We can add a name attribute to each element and let the handler function choose what to do based on the value of event.target.name. if we want to handle multiple controlled input elements.


# The Conditional (Ternary) Operator 

> it allows us to specify that a certain block of code should be executed if a certain condition is met, just like the if statment.

* the ternary operator help us to write a whole if statment code in just one line !

**here is the if statment we used to write and know** :

if ( condition ) {
  value if true;
} else {
  value if false;
}

**and here in the ternary operator code** :

condition ? value if true : value if false.