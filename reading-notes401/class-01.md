# class 1

## Readings: Node Ecosystem, TDD, CI/CD

CI/CD: software engineering, CI/CD or CICD is the combined practices of continuous integration and either continuous deployment or continuous deployment. CI/CD bridges the gaps between development and operation activities and teams by enforcing automation in building, testing and deployment of applications.

CI: continuous integration is the process of verifying that a software project is ready for deployment. Continuous integration is a process of verifying that a software project is ready for deployment. CI/CD is a combination of continuous integration and continuous deployment.

CD: continuous deployment is the process of delivering software to a customer. Continuous deployment is a process of delivering software to a customer. CI/CD is a combination of continuous integration and continuous deployment.

TDD: Test-driven development is a software development process relying on software requirements being converted to test cases before software is fully developed, and tracking all software development by repeatedly testing the software against all test cases.

## Review, Research, and Discussion

- Describe (in plain English) what Array.map() does:
  - map() is a method that takes a function and a list as arguments.
    - map() will apply the function to each element of the list and return a new list with the results.
- Describe (in plain English) what Array.reduce() does:
  - reduce() is a method that takes a function and a list as arguments.
    - reduce() will apply the function to each element of the list and return a single value.
- Provide code snippets showing how to use superagent() to fetch data from a URL and log the result:
  - With normal Promise .then() syntax:
    - superagent.get('https://api.github.com/users/jaredpalmer/repos')
      .then(function(response) {
      console.log(response.body);
      });
  - Again with async / await syntax:
    - const response = await superagent.get('https://api.github.com/users/jaredpalmer/repos');
    - console.log(response.body);
- Explain promises as though you were mentoring a Code 301 level student:
  - Promises are a way to handle asynchronous code.
- Are all callback functions considered to be Asynchronous? Why or Why Not?:
  - Yes, all callback functions are considered to be asynchronous.
