# Reading: Advanced State with Reducers

## Review, Research, and Discussion

- How can we ensure that an effect hook runs only once? dependance []
- Can useState() update more than one state variable at the same time? no
- Is useState() synchronous? yes

## Document the following Vocabulary Terms?|

| Term                | def                                                                                                                                                                                         |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| State Hook          | A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components. We'll learn other Hooks later. |
| Component Lifecycle | Each component in React has a lifecycle which you can monitor and manipulate during its three main phases. The three phases are: Mounting, Updating, and Unmounting.                        |

## Preparation Materials

- [useReducer hook](https://reactjs.org/docs/hooks-reference.html)
- [Ultimate Guide to useReducer](https://blog.logrocket.com/guide-to-react-usereducer-hook/)

useReducer is one of the additional Hooks that shipped with React 16.8. An alternative to the useState Hook, it helps you manage complex state logic in React applications. When combined with other Hooks like useContext, useReducer can be a good alternative to Redux or MobX — indeed, it can sometimes be an outright better option.

useReducer is used to store and update states, just like the useState Hook. It accepts a reducer function as its first parameter and the initial state as the second.

useReducer returns an array that holds the current state value and a dispatch function, to which you can pass an action and later invoke. This is similar to the pattern Redux uses but with a few differences.

For example, the useReducer function is tightly coupled to a specific reducer. We dispatch action objects to that reducer only, whereas in Redux, the dispatch function sends the action object to the store. At the time of dispatch, the components don’t need to know the reducer that will process the action.
