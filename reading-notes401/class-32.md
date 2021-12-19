# Reading: Context API - Behaviors

## Review, Research, and Discussion

- When you have multiple contexts, what component type should you use (class/function) and why?
  - Class:
    - It's a good practice to use a class for a component that has multiple contexts.
- What are some good use cases for using the Context API for global state?
  - It's a good practice to use the Context API for global state.
  - auth state
- How can you best test context?
  - The best way to test Context is to make our tests unaware of its existence and avoiding mocks. We want to test our components in the same way that developers would use them (behavioral testing) and mimic the way they would run in our applications (integration testing).

## Document the following Vocabulary Terms

| Term                                                                                                                                                                                                                                                                    | definitions                                                                                                                                                                                                                                             |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| context                                                                                                                                                                                                                                                                 | The Context API is a React structure that enables you to exchange unique details and assists in solving prop-drilling from all levels of your application.                                                                                              |
|                                                                                                                                                                                                                                                                         |
| useContext()                                                                                                                                                                                                                                                            | “useContext” hook is used to create common data that can be accessed throughout the component hierarchy without passing the props down manually to each level. Context defined will be available to all the child components without involving “props”. |
| static context                                                                                                                                                                                                                                                          | What is static context?                                                                                                                                                                                                                                 |
| A static method or, block belongs to the class and these will be loaded into the memory along with the class. You can invoke static methods without creating an object. ... But static contexts(methods and blocks) doesn't have any instance they belong to the class. |

## Preparation Materials

- [context api](https://reactjs.org/docs/context.html)
- [hooks and context example](https://medium.com/swlh/snackbars-in-react-an-exercise-in-hooks-and-context-299b43fd2a2b)
- [react context links](https://github.com/diegohaz/awesome-react-context)
