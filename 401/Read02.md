## Unit Testing Best Practices
- unit tests isolate and exercise specific units of code (ex: in C# a unit would be a method)
  - a unit test would test functionality of one specific method in isolation
- use a 'unit test project' template, located under test templates when creating a new project
- test calls the method with given inputs, then checks to see if the output is equal to the expected output and throws an error if it doesn't
- Assertion classes pass or fail
- base on the scientific method
- one assert per test
- tests should function independent of each other

## Art of README
- README should: tell someone what your program is, show them what it does, tell them how to use it
- short as possible
- project should be usable without having to view code
- Should include:
  - name
  - description (one line)
  - usage
  - API
  - installation
  - license
