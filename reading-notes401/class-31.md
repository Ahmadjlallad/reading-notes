# Reading: Context API

## Review, Research, and Discussion

In your reading notes page for this class, provide answers to the following prompts. Cite any external sources

- Describe use cases useState() vs useReducer()

  - useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.

- Why do custom hooks need the use prefix?

  - In other words, it's just like a normal function. Its name should always start with use so that you can tell at a glance that the rules of Hooks apply to it.

- What do custom hooks usually do?
  - Custom hooks allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks.
- Using any list of custom hooks, research and name one that you think will be useful in your applications
  - useEffect
- Describe how a hook that fetches API data might work

  - useEffect is a hook that runs after the component mounts. It's a great way to fetch data from an API or to update the DOM.

## Document the following Vocabulary Terms

| Term    | Definition                                                                                                                                                                                                                                                  |
| ------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| reducer | Introduction. In Redux, a reducer is a pure function that takes an action and the previous state of the application and returns the new state. The action describes what happened and it is the reducer's job to return the new state based on that action. |

## Preparation Materials

- [context api](https://reactjs.org/docs/context.html)

  - In a typical React application, data is passed top-down (parent to child) via props, but such usage can be cumbersome for certain types of props (e.g. locale preference, UI theme) that are required by many components within an application. Context provides a way to share values like these between components without having to explicitly pass a prop through every level of the tree.

- [hooks and context example](https://medium.com/swlh/snackbars-in-react-an-exercise-in-hooks-and-context-299b43fd2a2b)

  - From an engineering standpoint, our snackbar system must easy to use and generally be very lightweight. We want to be able to place one on the screen with just a couple of lines of code. Anything more and it’s overkill.
    This means forget render props and higher order components. We don’t want to deal with a messy React tree and wrappers. We don’t want action creators, reducers\*, or any of that stuff.
    Hooks are a perfect fit here. So lets imagine we have a custom hook that lets us do this and work backwards.
  - Globally Accessible
  - Sprinkling in Optimizations

- [react context links](https://github.com/diegohaz/awesome-react-context)
