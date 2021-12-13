# Reading: <Login /> and <Auth />

## Review, Research, and Discussion

- Why is the Context API useful?

  - The Context API is a React structure that enables you to exchange unique details and assists in solving prop-drilling from all levels of your application.

- Can a component outside of a provider get its context?
  - To access a React context outside of the render function, we can use the useContext hook.
- What are some common use cases for using the Context API?
  - Theming — Pass down app theme.
  - i18n — Pass down translation messages.
  - Authentication — Pass down current authenticated user. -
- Describe “Context Hell”
  - the nasty code you get taking advantage of the React Context API

## Document the following Vocabulary Terms

| Term           | definition                                                                                                                                                                       |
| -------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| global state   | To put it simply, global state is the data that is shared between all the components within a React application.                                                                 |
| global context | This global context is about how concerned we are worldwide, how we make decisions about global issues and how we can act in a responsible way to make the world a better place. |
| provider       | The Provider component accepts a value prop to be passed to consuming components that are descendants of this Provider. One Provider can be connected to many consumers.         |

| consumer | A React component that subscribes to context changes. |

## Preparation Materials

- [what is role based access control?](https://digitalguardian.com/blog/what-role-based-access-control-rbac-examples-benefits-and-more)

  - Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.
    Employees are only allowed to access the information necessary to effectively perform their job duties. Access can be based on several factors, such as authority, responsibility, and job competency. In addition, access to computer resources can be limited to specific tasks such as the ability to view, create, or modify a file.



- [react-cookies component](https://www.npmjs.com/package/react-cookies)
- [react-cookie library](https://www.npmjs.com/package/react-cookie)
