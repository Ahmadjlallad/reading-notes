# React

How would you break a mock into a component hierarchy?

- Use a component composition pattern single responsibility principle

  - What is the single responsibility principle and how does it apply to components?

    - What does it mean to build a ‘static’ version of your application?that is, a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.

  - Once you have a static application, what do you need to add?What are the three questions you can ask to determine if something is state?

    - Is it passed in from a parent via props? If so, it probably isn’t state.
    - Does it remain unchanged over time? If so, it probably isn’t state.
    - Can you compute it based on any other state or props in your component? If so, it isn’t state.

  - How can you identify where state needs to live?
    - identify every component that renders something based on that state.
    - Find a common owner component (a single component above all the components that need the state in the hierarchy).
    - Either the common owner or another component higher up in the hierarchy should own the state.
    - SIf you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

## Things I want to know more about

More React 🙌🐱‍👓
