# class 27 hooks

- How does React differ from vanilla JS/HTML/CSS?
  - React is a library that allows us to write components
- What is the primary difference between a function component and a class component?
  - A class component is a component that has a render method
  - A function component is a component that does not have a render method
- What is the difference between a stateless functional component and a class component?

  - A stateless functional component is a component that does not have a render method
  - A class component is a component that has a

## def

| Term                        | feg                                                                                                                                                                                                                                                                                                   |
| --------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Functional Components       | Functional components are functions that takes in props and return JSX. They do not natively have state or lifecycle methods, but this functionality can be added by implementing React Hooks. Functional components are usually used to display information. They are easy to read, debug, and test. |
| Children / Child Components | A parent component is a component that has a wider scope and a child component is a component that is apart of that scope but not all of it. One example is an html page that has a toolbar, a content area and a table inside the content area.                                                      |

Preview
Skim the following materials in preparation for the upcoming lecture. Note the following as you browse the material, and be prepared to participate in discussions during lecture

## Preparation Materials

- making sense of hooks
  - We know that components and top-down data flow help us organize a large UI into small, independent, reusable pieces. However, we often can’t break complex components down any further because the logic is stateful and can’t be extracted to a function or another component. Sometimes that’s what people mean when they say React doesn’t let them
- the state hook
  - What is a Hook? A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components. We’ll learn other Hooks later
