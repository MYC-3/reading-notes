# States and Props

## React
[Notes taken from here](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?
  - The render happens first.
2. What is the very first thing to happen in the lifecycle of React?
  - Mounting is the first phase and the constructor is the first occurs first in the mounting phase.
3. Put the following things in the order that they happen: `componentDidMount`, `render`, `constructor`, `componentWillUnmount`, `React Updates`
  - `constructor`, `render`, `react update`, `componentDidMount`, `componentWillUnmount`
4. What does componentDidMount do?
  - Used to load network requests or initialize the DOM.
  - Used to connect to API's.

[Following questions were answered using this video](https://www.youtube.com/watch?v=IYvD9oBCuJI)

1. What types of things can you pass in the props?
  - Similar to arguments in a function.
  - Numbers (for example, a counter functions initial count value)
  - Text (Title or subtitle to a page)
2. What is the big difference between props and state?
  - States are handled and updated within a component.
  - Props are handled and updated outside of a component and must be passed in.
3. When do we re-render our application?
  - When a state is changed
4. What are some examples of things that we could store in state?
  - Updating values based on user input, for example a form or counter.


[Back to HOME](../README.md)