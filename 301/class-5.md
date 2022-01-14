# Putting it all Together

## Thinking in React

- What is the single responsibility principle and how does it apply to components?
  - The single responsibility principle is the idea that one componenet should only do one thing
- What does it mean to build a ‘static’ version of your application?
  - Building a static version means to create a base version with no interactivity, eg don't implement state yet.
- Once you have a static application, what do you need to add?
  - If you make a change to the data or components and want to see it rendered you can call ReactDOM.render()
- What are the three questions you can ask to determine if something is state?
  - Is it passed in from parent via props? If so its probably not state.
  - Does it remain unchanged over time? If so, it probably isn't state
  - Can you compute it based on any other state or props in your component? If so, it isn't state.
- How can you identify where state needs to live?
  - Identify every component that renders based on state
  - Find a common parent component that is shared by all the state rendering child compoenents

## Higher Order Functions

- What is a “higher-order function”?
  - A higher order function is a function that takes callback functions, or returns another function inside of it
- Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?
  - greaterThan allows a new function to be saved to it, passing in the number that is to be the basis of comparison.
- Explain how either map or reduce operates, with regards to higher-order functions.
  - Map functions can be used as a callback, that take another callback function which determines what it should do to each el it returns. 
