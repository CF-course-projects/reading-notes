# State and Props

### What are life cylce events?
### Life cycle events are the methods that you are able to use on components

- Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?
  - render occurs before the componentDidMount
- What is the very first thing to happen in the lifecycle of React?
  - An instance of a component is created in the constructor 
- Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates
  - 1st: constructor, 2nd: render, 3rd: React updates, 4th: componentDidMount
- What does componentDidMount do?
  - This method is immediately invoked after a component is mounted, it is used for network requests and DOM manipulations.

### React State Vs Props

### If data is handled soley in a component and not outside of it, state is appropriate, if data is handled outside of a component, then props are passed to the component

- What types of things can you pass in the props?
  - props can pass data of all types
- What is the big difference between props and state?
  - props are passed into a component as arguements, whilst state is handled inside the component; props must be updated outside of the component, state can be updated within the component.
- When do we re-render our application?
  - We re-render our application when changes have been copied from the virtual DOM to the acutal DOM
- What are some examples of things that we could store in state?
  - Examples include form inputs, data changes, or dynamic functionalities
