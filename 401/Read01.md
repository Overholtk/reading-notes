
## Debugging for Absolute Beginners
- Debugging: run code step by step to find the exact point of mistake
- Ask yourself what you expected your code to do, and what it did instead
- Check that your data/API/API usage is correct
- Search for any typos
- Make sure you know the intent of the code
- Step through the code in debugging mode to pinpoint the problem
- Breakpoints indicate a pausing point to track individual steps

## Try/Catch Blocks
- Code that may raise or throw an exception should be encased in a try block
- Code used to handle the exceptions should be placed in a catch block
- Each catch block contains the exception type and statements to handle that type

## Statement Keywords
- Statements are program instructions
- Statements are usually run in sequence
- Statement keywords can alter the order statements will run in
  - (ex: in a series of if statements, only the statements that resolve as true will run, taking them out of their written order.)
  
## Therac-25
- Therac-25 was a computer controlled radiation machine
- Overdosed patients with considerable amounts of radiation due to programming errors
- Software was poorly designed and difficult to test in a clean way
- Code was not independently reviewed
- Unadressed and vague error codes
- High volume of errors caused operators to go on autopilot when addressing
- No backup hardware locks

## Ariane 5
- European spacecraft
- Rocket self destructed 37 seconds after launch due to software on first test flight (6/4/96)
- data conversion from 64-bit to 16-bit
- variable was unprotected to minimize workload
