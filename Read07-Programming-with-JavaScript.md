#### Programming with JavaScript
- Control flow: is the order in which the computer executes statements in a script.
  - Js run in order from the first line in the file to the last line.
    - but there are some structures can change this flow such as conditionals and loops, this cass can happen when a web page need the user to fill up from for example:
       ```if (field==empty) {
      promptUser();
      } else {
      submitForm();
      }. 
    ```
### Functions: 
- Functions are one of the fundamental building blocks in JavaScript, set of statements that performs a task or calculates a value, it should take some input and return an output where there is some obvious relationship between the input and the output.
  - Defining functions: 
    - function declaration by using ```function``` followed by name of the function ofcorse here function return a value to the parameter or between brackets in this example this parameter called number, return: return value to the parameter.
      ```function square(number) {return number * number;}```

    - anonymous declaration: Providing a name allows the function to refer to itself.
    ``` anonymous declaration
    const factorial = function fac(n) { return n < 2 ? 1 : n * fac(n - 1) }
    console.log(factorial(3))
    ```
  
  - Calling functions: from above example calling ```square(arguments)``` arguments should be included
    - Function call it self "recursive function"
      clever example 
      ``` clever example 
        function factorial(n) {
      if ((n === 0) || (n === 1))
        return 1;
      else
        return (n * factorial(n - 1));}
        ```
      in this example if you pass `console.log(factorial(5))` you will get 120 
      `return (n * factorial(n - 1))` keep executes until `n` becomes `1`.
  - Function scope: Variables  that got defined in the function scope will not accessed     from anywhere outside the function.
    - Recursion: A function can refer to and call itself.in the below example `foo()` repet it self evre time function get called.
      ```
      function foo(i) {
      if (i < 0)
        return;
      console.log('begin: ' + i);
      foo(i - 1);
      console.log('end: ' + i);}foo(3); 
      ```
    - Nested functions and closures:  nest a function within another function. The nested (inner) function is private to its containing (outer) function, but inner function can access outer function variables.
    - Since the inner function forms a closure, you can call the outer function and specify arguments for both the outer and inner function:
    - Closures: allows for the nesting of functions and grants the inner function full access to all the variables and functions defined inside the outer function
    - similar to Object Oriented Programming .
```
Object Oriented Programming 
var createPet = function(name) {
var sex;

return {
setName: function(newName) {
name = newName;
},

getName: function() {
return name;
},

getSex: function() {
return sex;
},

setSex: function(newSex) {
if(typeof newSex === 'string' && (newSex.toLowerCase() === 'male' ||
newSex.toLowerCase() === 'female')) {
sex = newSex;
}
}
}
}

var pet = createPet('Vivie');
pet.getName();                  

pet.setName('Oliver');
pet.setSex('male');
pet.getSex();                   
pet.getName();              
```
###### Hope you had fun
