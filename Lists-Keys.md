# Lists

> Building collection of elements using curly braces, we loop into the array and then we use map() function and return the array between  <li> elements.

> Usually you would render lists inside a component.

# Keys:

> Its a way to identify which items have changed, are added, or are removed, Keys should be given to the elements inside the array to give the elements a stable identity.

*  we use the item index as a key When we don’t have stable IDs for rendered items.

*  keys don’t need to be globally unique. We can use the same keys when we produce two different arrays.

# The spread operator :

> its a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.

**spread operator is useful for many different routine tasks in JavaScript such as**

* Using Math functions.

* Using an array as arguments

* Adding an item to a list

* Adding to state in React

### here is an example of the speared operator to combine two arrays

 
const fruits = ['🍏','🍊','🍌','🍉','🍍']
const moreFruits = [...fruits];
console.log(moreFruits) // Array(5) [ "🍏", "🍊", "🍌", "🍉", "🍍" ]
fruits[0] = '🍑'
console.log(...[...fruits,'...',...moreFruits]) //  🍑 🍊 🍌 🍉 🍍 ... 🍏 🍊 🍌 🍉 🍍

" code taking from https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab "


###  an example of the speared operator to add a new item to an array


const fewFruit = ['🍏','🍊','🍌']
const fewMoreFruit = ['🍉', '🍍', ...fewFruit]
console.log(fewMoreFruit) //  Array(5) [ "🍉", "🍍", "🍏", "🍊", "🍌" ]

" code taking from https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab "


### an example of the speared operator to combine two objects into one.

const objectOne = {hello: "🤪"}
const objectTwo = {world: "🐻"}
const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
objectFour.laugh() // 😂😂😂😂😂

" code taking from https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab "


