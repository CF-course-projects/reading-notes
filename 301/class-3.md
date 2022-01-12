# Passing Functions as Props

## React Docs - lists and keys

- What does .map() return?
  - .map() returns an array of elements.
- If I want to loop through an array and display each value in JSX, how do I do that in React?
  - To do so in React, we can save the return value of calling the map method on the array in question and instantiate elements, inserting elements of the array within the map function
- Each list item needs a unique ____.
  - key.
- What is the purpose of a key?
  - The purpose of keys is to help React keep track of which itmes have changed, are added or are removed.

## The Spread Operator

- What is the spread operator? 
  - The spread operator is used when passing in arrays into functions that take only one argument. The spread operator feeds the function one element of the array at a time
- List 4 things that the spread operator can do.
- Give an example of using the spread operator to combine two arrays.
- Give an example of using the spread operator to add a new item to an array.
- Give an example of using the spread operator to combine two objects into one.

## How to Pass Functions Between Components

- In the video, what is the first step that the developer does to pass functions between components?
  - The developer passes the function to the child component via props and referencing this.functionName
  - Ex: function = {this.functionName}
- In your own words, what does the increment function do?
  - The increment function updates the state object, more specifically updates the people array via map method
- How can you pass a method from a parent component into a child component?
  - You can pass a method from a parent component to child via props in the child component invocation
- How does the child component invoke a method that was passed to it from a parent component?
  - A child component can call a method passed to it by using: this.props.methodName()
