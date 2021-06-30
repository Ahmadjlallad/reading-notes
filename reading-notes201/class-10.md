#JS

## ERRORS

##### ORDER OF EXECUTION

- some tasks cannot complete until another statement or function has been run

##### EXECUTION CONTEXT JavaScript

- Every statement in a script lives in one of three
  execution contexts:
- There is only one global context in any page
- FUNCTION CONTEXT
- EVAL CONTEXT (NOT SHOWN),Text is executed like code in an internal function called eva l {)

##### EXECUTION CONTEXT & HOISTING

there are two phases of activity

- PREPARE create every thing and determined this keyword
- EXECUTE

##### UNDERSTANDING SCOPE

In the interpreter, each execution context has its own va ri ables object.
It holds the variables, functions, and parameters available within it.
Each execution context can also access its parent's v a ri ables object.

##### UNDERSTANDING ERRORS

- If a JavaScript statement generates an error, then it throws an exception.
  At that point, the interpreter stops and looks for exception-handling code.

##### ERROR OBJECTS

Error objects can help you find where your mistakes are and browsers have tools to help you read them.

##### HOW TO DEAL WITH ERRORS

- DEBUG THE SCRIPT TO FIX ERRORS

- HANDLE ERRORS GRACEFULLY: error beyond your control.

  - WHERE IS THE PROBLEM?
    - Look at the error message
    - Check how far the script is running
    - Use breakpoints where things are going wrong

##### BREAKPOINTS

- You can pause the execution of a script on any line using breakpoints. Then you can check the values stored in variables at that point in time.

##### STEPPING THROUGH CODE

-If you set multiple breakpoints, you can step through them one-by-one to see where values change and a problem might occur

##### CONDITIONAL BREAKPOINTS

- You can indicate that a breakpoint should be triggered only if a condition that you specify is met. The condition can use existing variables.

##### DEBUGGER KEYWORD

- You can create a breakpoint in your code using just the debugger keyword. When the developer tools are open, this will automatically create a breakpoint.

##### HANDLING EXCEPTIONS

```js
try {
  // Try to execute this code
} catch (exception) {
  // If there is an exception, run this code
} finally {
  // This always gets executed
}
```

- First, you specify the code that you think might throw an exception within the try block

- If the try code block throws an exception, catch steps in with an alternative set of code . It has one parameter

- The contents of the finally code block will run either way whether the try block succeeded or failed.

##### THROWING ERRORS

- If you know something might cause a problem for your script, you can generate your own errors before the interpreter creates them.
  `throw new Error(message 1) ;`

##### DEBUGGING TIPS

- EXPLAINING THE CODE
- CODE PLAYGROUNDS
- SEARCH
