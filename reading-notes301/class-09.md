# [Functional Programming Concepts](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

- What is functional programming?

  - Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data — Wikipedia

- What is a pure function and how do we know if something is a pure function?
  - It returns the same result if given the same arguments (it is also referred as deterministic)
  - It does not cause any observable side effects
- What are the benefits of a pure function?
  - It is easier to test, The code’s definitely easier to test. We don’t need to mock anything
- What is immutability?

  - state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

- What is Referential transparency?

  - it can be replaced with its corresponding value (and vice-versa) without changing the program's behavior
    `pure functions + immutable data = referential transparency`

## [Node Modules](https://www.youtube.com/watch?v=xHLd36QoS4k)

- What is a module?
  - simple or complex functionality organized in single or multiple JavaScript files which can be reused throughout the Node
- What does the word ‘require’ do?
  - used to load and cache JavaScript modules
- How do we bring another module into the file the we are working in?
  - `module.exports = { your function };`
- What do we have to do to make a module available?
  - require("your file path");
