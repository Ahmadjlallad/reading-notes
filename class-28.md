# class 28 Reading: Component Lifecycle / useEffect() Hook

## Review, Research, and Discussion

In your reading notes page for this class, provide answers to the following prompts. Cite any external sources

- Why do we not need more .html pages in a multi-page React app?
  -Using the react-router-dom package, we can implement multiple routes in a React application. A user browsing this app feels each route is on each page. So in React, multiple routes are considered as multiple pages.
- If we wanted a component to show up on every page, where would we put it and why?
  - Outside the <BrowserRouter/>
  - Inside the <BrowserRouter />, outside a <Route />
  - Inside a <Route />
  - Inside BrowserRouter and inside a Route ✔️
- What does routing do with the components that were rendered when a new route is requested
  - One way to do would be to pass the component prop an inline function. When you use component, the router uses React. createElement to create a new React element from the given component. That means if you provide an inline function to the component prop, you would create a new component every render.
- What does props.children contain?
  - props. children does is that it is used to display whatever you include between the opening and closing tags when invoking a component. This component contains an <img> that is receiving some props and then it is displaying {props. children}
- How do useState() and this.setState() differ?

  - setState() does not immediately mutate this. state but creates a pending state transition. Accessing this. state after calling this method can potentially return the existing value.

  ## Document the following Vocabulary Terms

  | Term                     | def                                                                                                                                                                                                                                                                                         |
  | :----------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
  | State Hook               | In a function component, we have no this, so we can’t assign or read this.state. Instead, we call the useState Hook directly inside our component                                                                                                                                           |
  | Mounting and Un-Mounting | The main job of React is to figure out how to modify the DOM to match what the components want to be rendered on the screen. React does so by "mounting" (adding nodes to the DOM), "unmounting" (removing them from the DOM), and "updating" (making changes to nodes already in the DOM). |

  ## Preview

Skim the following materials in preparation for the upcoming lecture. Note the following as you browse the material, and be prepared to participate in discussions during lecture
[effects hook](https://reactjs.org/docs/hooks-effect.html)
