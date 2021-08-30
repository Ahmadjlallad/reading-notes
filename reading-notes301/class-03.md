# check out my react web app deployed on github pages

## [Videos-App](https://ahmadjlallad.github.io/Videos-App/)

## [Search Images](https://ahmadjlallad.github.io/learningReact/)

## React

- What is the purpose of a key? A “key” is a special string attribute you need to include when creating lists of elements in React. Keys are used to React to identify which items in the list are changed, updated, or deleted. In other words, we can say that keys are used to give an identity to the elements in the lists.

Videos: [How to Pass Functions Between Components](https://www.youtube.com/watch?v=c05OL7XbwXU)

- In the video, what is the first step that the developer does to pass functions between components?
  - The first step is to pass the function as a prop to the component.
- In your own words, what does the increment function do?
  - The increment function is used to increment the state of the counter.
- How can you pass a method from a parent component into a child component?
  - You can pass a method from a parent component into a child component by using the props.
- How does the child component invoke a method that was passed to it from a parent component?
  - The child component can invoke a method that was passed to it from a parent component by using the props.

## The Spread Operator

- `...` is the spread operator. It allows us to expand the contents of an array into a list of elements.
- List 4 things that the spread operator can do?

  - Copying an array.
  - Concatenating or combining arrays.
  - Using Math functions.
  - Using an array as arguments.

- Give an example of using the spread operator to combine two arrays.

```Js
const arr1 = [1,2,3]
const arr2 = [4,5,6]
const arr3 = [...arr1, ...arr2]
```

- Give an example of using the spread operator to add a new item to an array

```js
const odd = [1, 3, 5];
const combined = [2, 4, 6, ...odd];
```

- Give an example of using the spread operator to combine two objects into one.

```js
const person = {
  firstName: "John",
  lastName: "Doe",
  age: 25,
  ssn: "123-456-2356",
};

const job = {
  jobTitle: "JavaScript Developer",
  location: "USA",
};

const employee = {
  ...person,
  ...job,
};
```

## Things I want to know more about

- Redux
