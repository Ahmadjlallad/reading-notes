# Readings: Redux - Asynchronous Actions

## Review, Research, and Discussion

- How granular should your reducers be?
  - As of 2020, we specifically recommend putting as much logic as possible in reducers: Wherever possible, try to put as much of the logic for calculating a new state into the appropriate reducer, rather than in the code that prepares and dispatches the action (like a click handler).
- Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched
  - Dispatching an action within a reducer is an anti-pattern.

Your reducer should be without side effects, simply digesting the action payload and returning a new state object. Adding listeners and dispatching actions within the reducer can lead to chained actions and other side effects.

- Name a strategy for preventing the above
  Step 1: identifying hazards and those at risk.
  Step 2: evaluating and prioritising risks.
  Step 3: Deciding on preventive action.
  Step 4: Taking action.
  Step 5: Monitoring and reviewing.

## Document the following Vocabulary Terms

| Term              | def                                                                                                                                                                                                                                                                    |
| ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| store             | A store is an immutable object tree in Redux. A store is a state container which holds the application's state. Redux can have only a single store in your application. Whenever a store is created in Redux, you need to specify the reducer.                         |
| combined reducers | The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore . The resulting reducer calls every child reducer, and gathers their results into a single state object. |

## Preparation Materials

- [async actions](https://redux.js.org/tutorials/fundamentals/part-6-async-logic)
- [thunk middleware](https://github.com/reduxjs/redux-thunk)
- [redux thunk](https://www.digitalocean.com/community/tutorials/redux-redux-thunk)
