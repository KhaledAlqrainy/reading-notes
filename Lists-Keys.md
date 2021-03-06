# Lists

> Building collection of elements using curly braces, we loop into the array and then we use map() function and return the array between  <li> elements.

> Usually you would render lists inside a component.

# Keys:

> Its a way to identify which items have changed, are added, or are removed, Keys should be given to the elements inside the array to give the elements a stable identity.

*  we use the item index as a key When we donβt have stable IDs for rendered items.

*  keys donβt need to be globally unique. We can use the same keys when we produce two different arrays.

# The spread operator :

> its a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a functionβs arguments.

**spread operator is useful for many different routine tasks in JavaScript such as**

* Using Math functions.

* Using an array as arguments

* Adding an item to a list

* Adding to state in React

### here is an example of the speared operator to combine two arrays

 
const fruits = ['π','π','π','π','π']
const moreFruits = [...fruits];
console.log(moreFruits) // Array(5) [ "π", "π", "π", "π", "π" ]
fruits[0] = 'π'
console.log(...[...fruits,'...',...moreFruits]) //  π π π π π ... π π π π π

" code taking from https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab "


###  an example of the speared operator to add a new item to an array


const fewFruit = ['π','π','π']
const fewMoreFruit = ['π', 'π', ...fewFruit]
console.log(fewMoreFruit) //  Array(5) [ "π", "π", "π", "π", "π" ]

" code taking from https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab "


### an example of the speared operator to combine two objects into one.

const objectOne = {hello: "π€ͺ"}
const objectTwo = {world: "π»"}
const objectThree = {...objectOne, ...objectTwo, laugh: "π"}
console.log(objectThree) // Object { hello: "π€ͺ", world: "π»", laugh: "π" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("π".repeat(5))}}
objectFour.laugh() // πππππ

" code taking from https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab "


