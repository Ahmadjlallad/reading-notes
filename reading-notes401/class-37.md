# Readings: Redux - Combined Reducers

## Review, Research, and Discussion

In your reading notes page for this class, provide answers to the following prompts. Cite any external sources

- Why choose Redux instead of the Context API for global state?
  - Context API is easy to is use as it has a short learning curve. It requires less code, and because there's no need of extra libraries, bundle sizes are reduced. Redux on the other hand requires adding more libraries to the application bundle. The syntax is complex and extensive creating unnecessary work and complexity.
- What is the purpose of a reducer?
  - A reducer is a function that determines changes to an application's state. It uses the action it receives to determine this change. We have tools, like Redux, that help manage an application's state changes in a single store so that they behave consistently.
- What does an action contain?
  - Actions are the only source of information for the store as per Redux official documentation.
- Why do we need to copy the state in a reducer?
  - If the new state is different, the reducer must create new object, and making a copy is a way to describe the unchanged part.

## Document the following Vocabulary Terms

| Term                 | def                                                                                                                                                                                                                                                                                  |
| -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| immutable state      | Immutability is a concept that React programmers need to understand. An immutable value or object cannot be changed, so every update creates new value, leaving the old one untouched                                                                                                |
| time travel in redux | Redux refers to the process of logging actions and state during an app's execution. Since it represents the entire state of an application at a given moment, it is often used in web development for time-travel debugging and to view Redux actions.                               |
| action creator       | An action creator is a function that literally creates an action object. In Redux, action creators simply return an action object and pass the argument value if necessary.                                                                                                          |
| reducer              | A reducer is a very simple idea and it's something that will be easy for you to grasp because, in a nutshell, it's just a simple JS function. A reducer is a function which takes two arguments — the current state and an action — and returns based on both arguments a new state. |
| dispatch             | dispatch is a function of the Redux store. You call store. dispatch to dispatch an action. This is the only way to trigger a state change. With React Redux, your components never access the store directly - connect does it for you.                                              |
|                      |

## Preparation Materials

- [Multiple Reducers Example](https://www.youtube.com/watch?v=gBER4Or86hE)
- [Redux Docs: Using Combined Reducers](https://redux.js.org/usage/structuring-reducers/using-combinereducers/)
- [Redux Docs: Combined Reducer Syntax](https://redux.js.org/api/combinereducers/)
