# Passing Functions as Props

1- What does .map() return?

    Map function it return array

2- If I want to loop through an array and display each value in JSX, how do I do that in React?

    array.map((callback))

3- Each list item needs a unique ***key***.

4- What is the purpose of a key?

    Keys should be given to the elements inside the array to give the elements a stable identity.

# How to Use the Spread Operator (…) in JavaScript

1-  What is the spread operator?

    The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.


2- List 4 things that the spread operator can do.

    *  Copying an array
    * Concatenating or combining arrays
    * Using Math functions
    * Using an array as arguments

3- Give an example of using the spread operator to combine two arrays.

    const arrayOne=['A','B']
    const arrayTwo=['C','D']
    const bigArray=[...arrayOne,...arrayTwo]
    console.log(...bigArray)

4- Give an example of using the spread operator to add a new item to an array.

    const arrayOne=['A','B']
    const bigArray=[...arrayOne,'C','D']
    console.log(...bigArray)


5- Give an example of using the spread operator to combine two objects into one

    const user = {name: "Qasem"}
    const userId = {id: 5}

    const datauser = {...user,...userId}
    console.log(datauser);


1- In the video, what is the first step that the developer does to pass functions between components?

    create  anew function and use state and map function

2- In your own words, what does the increment function do?

    it will change value by state goals

3- How can you pass a method from a parent component into a child component?

    by using setstate

4- How does the child component invoke a method that was passed to it from a parent component?

    bu using super()

