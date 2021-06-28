# Passing Functions as Props

## Lists and Keys

We use the map() function to take an array of numbers and double their values.

Rendering Multiple Components You can build collections of elements and include them in JSX using curly braces {}.

Keys Must Only Be Unique Among Siblings Keys used within arrays should be unique among their siblings. However, they don’t need to be .

1-What does .map() return?
return new array

2-If I want to loop through an array and display each value in JSX, how do I do that in React?
We can build collections of elements and include them in JSX using curly braces and render it to the DOM.

3-Each list item needs a unique ____.

(KEY)

4-What is the purpose of a key?

A special string attribute you need to include when creating lists of elements .

![image](https://res.cloudinary.com/practicaldev/image/fetch/s--3CK7bFW5--/c_imagga_scale,f_auto,fl_progressive,h_500,q_auto,w_1000/https://dev-to-uploads.s3.amazonaws.com/i/4c7vey3xravg5egeow8t.png)

# The Spread Operator

1-What is the spread operator?
JavaScript, spread syntax refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.

2-List 4 things that the spread operator can do.
* Copying an array
* Concatenating or combining arrays
* Using Math functions
* Using an array as arguments
* Adding an item to a list
* Adding to state in React
* Combining objects
* Converting NodeList to an array

3-Give an example of using the spread operator to combine two arrays.
const myArray = [1,2,3] const yourArray = [4,5,6] const ourArray = […myArray,…yourArray] console.log(…ourArray) // 1 2 3 4 5 6

4-Give an example of using the spread operator to add a new item to an array.

const myArray = [‘1’,’2’,’3’] const moreArray = [‘4’, ‘5’, …moreNumbers] console.log(moreArray) // Array(5) [ “4”, “5”, “1”, “2”, “3” ]

5-Give an example of using the spread operator to combine two objects into one.

const objectOne = {hello: “🤪”} const objectTwo = {world: “🐻”} const objectThree = {…objectOne, …objectTwo, laugh: “😂”} console.log(objectThree) // Object { hello: “🤪”, world: “🐻”, laugh: “😂” } const objectFour = {…objectOne, …objectTwo, laugh: () => {console.log(“😂”.repeat(5))}} objectFour.laugh() // 😂😂😂😂😂

# How to Pass Functions Between Components
1-In the video, what is the first step that the developer does to pass functions between components?

Create a function wherever the state is that we are going to change.

2-In your own words, what does the increment function do?

Is recive an object , and loop inside the array using map method , then find the matching name and update the count by one

3-How can you pass a method from a parent component into a child component?

 using constructor keyword then spicify the methods using super method.

4-How does the child component invoke a method that was passed to it from a parent component?

 using the state method , it can from them invoke the method and update the component methods or attreputs.

 ![image](https://cdn-images-1.medium.com/fit/t/1600/480/1*TNZvScQmoS68ZJ9hbFXV8g.png)