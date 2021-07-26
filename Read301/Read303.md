# Passing Functions as Props

## Lists and Keys
 
## What does .map() return?

An Array containing the results of calling the provided function for each element in the original array.

## If I want to loop through an array and display each value in JSX, how do I do that in React?

we can loop through the array using the JavaScript map() function.and assign the resulting array of elements

map in JavaScript iterates through an array and calls a specified function for each of the items. Components in JSX are JS functions. For each object in the array, a block of JSX elements is returned.

## Each list item needs a unique ____.

The best way to pick a key is to use a string that uniquely identifies a list item among its siblings. Most often you would use IDs from your data as keys

## What is the purpose of a key?

Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity

# the Spread Operator

1- What is the spread operator?

InJavaScript, spread syntax refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.

The spread operator was added to JavaScript in ES6 (ES2015)

2- List 4 things that the spread operator can do.

1- Copying an array

2- Concatenating or combining arrays

3- Using Math functions

4- Using an array as arguments

5- Adding an item to a list

6- Adding to state in React

7- Combining objects

8- Converting NodeList to an array

3- Give an example of using the spread operator to combine two arrays.

>Ex :

const myArray = [`🤪`,`🐻`,`🎌`]

const yourArray = [`🙂`,`🤗`,`🤩`]

const ourArray = [...myArray,...yourArray]

console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩]

4- Give an example of using the spread operator to add a new item to an array.

>Ex :

const fruits = ['🍏','🍊','🍌','🍉','🍍']

const moreFruits = [...fruits];

console.log(moreFruits) // Array(5) [ "🍏", "🍊", "🍌", "🍉", "🍍" ]

fruits[0] = '🍑'

console.log(...[...fruits,'...',...moreFruits]) //  🍑 🍊 🍌 🍉 🍍 ... 🍏 🍊 🍌 🍉 🍍

5- Give an example of using the spread operator to combine two objects into one.

>Ex :
 
const objectOne = {hello: "🤪"}

const objectTwo = {world: "🐻"}

const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}

console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }

const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}

objectFour.laugh() // 😂😂😂😂😂

### for more ex visit this site [click here](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)


# Pass Functions Between Components

1- In the video, what is the first step that the developer does to pass functions between components?

Create a function in the parent component.

2- what does the increment function do?

It increments the count variablie and passed from the parent to the child by one

3- How can you pass a method from a parent component into a child component?

By sending it as a prop, and in the child component you can call inside another function and use stute inside the child 

4- How does the child component invoke a method that was passed to it from a parent component?

It invokes the method inside a method written inside of it, and if a parameter was a passed prop, you can call it