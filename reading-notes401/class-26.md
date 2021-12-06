# Reading: Component Based UI

## Review, Research, and Discussion

- Name 5 Javascript UI Frameworks (other than React)

  - AngularJS
  - Ember
  - Vue
  - Backbone
  - Knockout

- What’s the difference between a framework and a library?

  - A framework dose execute and use code we write, while a library does not.
  - but as a library, we use it in are code.

  ## Document the following Vocabulary Terms

  | Term      | doc                                                                                             |
  | --------- | ----------------------------------------------------------------------------------------------- |
  | Rendering | responsible for describing the view to be rendered to the browser window.                       |
  | Templates | templates are a way to display information on the user's browser.                               |
  | State     | the outcome of all of the actions that the user has taken since the page is loaded or rendered. |

## Preview

Skim the following materials in preparation for the upcoming lecture. Note the following as you browse the material, and be prepared to participate in discussions during lecture

- Which 3 things had you heard about previously and now have better clarity on?
  - react
  - components
  - state
- Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  - components
  - state
  - props
- What are you most excited about trying to implement or see how it works?
  - hokes

## Preparation Materials

- introducing JSX

  - React embraces the fact that rendering logic is inherently coupled with other UI logic: how events are handled, how the state changes over time, and how the data is prepared for display.

    Instead of artificially separating technologies by putting markup and logic in separate files, React separates concerns with loosely coupled units called “components” that contain both. We will come back to components in a further section, but if you’re not yet comfortable putting markup in JS, this talk might convince you otherwise.

    React doesn’t require using JSX, but most people find it helpful as a visual aid when working with UI inside the JavaScript code. It also allows React to show more useful error and warning messages.

- rendering elements

  - We call this a “root” DOM node because everything inside it will be managed by React DOM.

    Applications built with just React usually have a single root DOM node. If you are integrating React into an existing app, you may have as many isolated root DOM nodes as you like.

    To render a React element into a root DOM node, pass both to ReactDOM.render():
