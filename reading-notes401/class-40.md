# Reading: React Native

## Review the Submission Instructions for guidance on completing and submitting this assignment.

### Review, Research, and Discussion

- Compare and Contrast Redux Toolkit with Redux “Ducks”
  - The Redux Toolkit generates the new state from the direct changes to the old state. ... The reducers that are written with immer are 2 to 3 times slower than a normal Redux reducer. Here is an example of a Reducer function that uses the state as immutable and one which makes changes directly to the state.
- What is the principle advantage of Redux Toolkit
  - Redux Toolkit makes it easier to write good Redux applications and speeds up development

#### Document the following Vocabulary Terms

| Term                 | def                                                                                                                                                                                                   |
| -------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| redux toolkit slices | A function that accepts an initial state, an object of reducer functions, and a "slice name", and automatically generates action creators and action types that correspond to the reducers and state. |
| namespace            | In computing, a namespace is a set of signs (names) that are used to identify and refer to objects of various kinds.                                                                                  |

## Preview

### Skim the following materials in preparation for the upcoming lecture. Note the following as you browse the material, and be prepared to participate in discussions during lecture

#### Preparation Materials

- [getting started with react native](https://reactnative.dev/docs/getting-started)
- [react native basics (Tutorial)](https://reactnative.dev/docs/tutorial)
- [react native](https://reactnative.dev/)
- [expo](https://expo.dev/)
  - Expo is a framework and a platform for universal React applications. It is a set of tools and services built around React Native and native platforms that help you develop, build, deploy, and quickly iterate on iOS, Android, and web apps from the same JavaScript/TypeScript codebase.
- [expo snack](https://snack.expo.dev/)
  - Expo Snack is an open-source platform for running React Native apps in the browser.
- [ejecting](https://docs.expo.dev/expokit/eject/?redirected)
  - If you created an Expo project and you want a way to add custom native modules, this guide will explain how to use ExpoKit for that purpose.
    Normally, Expo apps are written in pure JS and never "drop down" to the native iOS or Android layer. This is core to the Expo philosophy and it's part of what makes Expo fast and powerful to use.
    However, there are some cases where advanced developers need native capabilities outside of what Expo offers out-of-the-box. The most common situation is when a project requires a specific Native Module which is not supported by React Native Core or the Expo SDK.
    In this case, Expo allows you to eject your pure-JS project from the Expo iOS/Android clients, providing you with native projects that can be opened and built with Xcode and Android Studio. Those projects will have dependencies on ExpoKit, so everything you already built will keep working as it did before.
    We call this "ejecting" because you still depend on the Expo SDK, but your project no longer lives inside Expo Go. You control the native projects, including configuring and building them yourself.
