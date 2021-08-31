# React Docs - Forms

- What is a ‘Controlled Component’?

  - controlled component is a component that renders form elements and controls them by keeping the form data in the component's state.

- Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

  - you should update the state with the users responses as soon as they enter them because it is a controlled component and as soon as the user enters their response, the component will update the state.

- How do we target what the user is entering if we have an event handler on an input field?

  - using event properties to target the input field.

- Why would we use a ternary operator?

  - Use the ternary operator to simplify your if-else statements that are used to assign values to variables. The ternary operator is commonly used when assigning post data or validating forms.

- Rewrite the following statement using a ternary statement:

```js
if (x === y) {
  console.log(true);
} else {
  console.log(false);
}
```

```js
x === y ? console.log(true) : console.log(false);
```

## Things I want to know more about

- redux
