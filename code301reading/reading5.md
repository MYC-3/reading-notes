# Putting it all Together

## Thinking in React
[All notes were taken from here](https://reactjs.org/docs/thinking-in-react.html)

- How would you break a mock into a component heirarchy?
  It easy to visualize the mock in components by drawing a box around every component.
- What is the **single responsibility principle** and how does it apply to components?
  A general rule that a single component should serve one purpose.
- What does it mean to build a ‘static’ version of your application?
  A model of your website/page that has no interactivity.
- Once you have a static application, what do you need to add?
  After building the static version, you should add interactivity and states.
- What are the three questions you can ask to determine if something is state?
>- Is it passed in from a parent via props? If so, it probably isn’t state.
>- Does it remain unchanged over time? If so, it probably isn’t state.
>- Can you compute it based on any other state or props in your component? If so, it isn’t state.
- How can you identify where state needs to live?
>- Identify every component that renders something based on that state.
>- Find a common owner component (a single component above all the components that need the state in the hierarchy).
>- Either the common owner or another component higher up in the hierarchy should own the state.
> -If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.
- A state should be in the lowest common component of all components that will use that state.

[Back to HOME](../README.md)