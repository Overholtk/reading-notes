# Refactoring

Functional Programming: A style of building the struture and elements of computer programs that treats the computation as the evaluation of mathematical functions and avoids changing state and mutable data

Pure Functions:
- Returns the same result if given the same arguments (deterministic)
  - Does not reference external objects (avoid using parameters)
  - Does not reference files
  - Does not reference randomly generated numbers
- Does not cause observable side effects
  - Does not modify a global object or a parameter

Immutability:
- Unchanging over time or unable to be changed
- state cannot change
- return a new variable or object instead
- function chaining: the result of a function will be used as the input for the next function, without modifying the original input

Referential transparency is a pure function using immutable data

Functions as first-class entities:
- can:
  - referto it from constants and variables
  - pass it as a parameter to other functions
  - return it as a result from other functions
- Higher-order functions:
  - takes one or more functions as arguments
  - returns a function as a result
-

