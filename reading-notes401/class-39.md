# Readings: Redux - Additional Topics

## Below you will find some reading material, code samples, and some additional resources that support today’s topic and the upcoming lecture.

### Review the Submission Instructions for guidance on completing and submitting this assignment.

#### Review, Research, and Discussion

In your reading notes page for this class, provide answers to the following prompts. Cite any external sources

- What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?
  - Answer. The most 'redux-like' way of handling the pre-loading of data would be to fire off the asynchronous action in the lifecycle method (probably componentWillMount ) of a Higher Order Component that wraps your app.
- When using a thunk/async action that dispatches the actual action, which do you export from your reducer?
  - To dispatch async actions into our store, we have to apply the thunk middleware by writing: const store = createStore(joke, applyMiddleware(thunk)); to apply the middleware. Then in App

#### Document the following Vocabulary Terms

| Term       | def                                                                                                                                                                                                                                        |
| ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| middleware | Redux middleware provides a third-party extension point between dispatching an action, and the moment it reaches the reducer. People use Redux middleware for logging, crash reporting, talking to an asynchronous API, routing, and more. |

|
|thunk|Redux Thunk is a middleware that allows you to call the action creators that return a function(thunk) which takes the store's dispatch method as the argument and which is afterwards used to dispatch the synchronous action after the API or side effects has been finished.|

#### Preparation Materials

- [Redux Toolkit (RTK)](https://redux-toolkit.js.org/introduction/getting-started)
- [Tutorial](https://redux-toolkit.js.org/tutorials/overview)
- Alternative State Managers

- [MobX](https://mobx.js.org/getting-started.html)
- [HookState](https://hookstate.js.org/)
