![](https://cdn.cnn.com/cnnnext/dam/assets/150103074330-hubble-space-background-2-large-169.jpg)

# Operators and Loops

## Comparison operators
- evaluate by comparing for a true or false boolean result
    - `==`: is equal to compares two values to determine if they are the same
    - `!=`: is not equal to will return true if the values are different
    - `===`: strict equal to determines if the values are exactly the same both in value and type
    - `!==`: strict not equal to will return false if either data type or value are different
    - `>`: greater than checks if the number on the left is greater than the number on the right
    - `>=`: greater than or equal to checks if the number on the left is of greater or equal value to the right
    - `<`: less than determines if the number on the left is smaller than the number on the right
    - `<=` less than or equal to determines if the number on the left is lesser or equal to the number on the right

## Logical Operators
- allows to compare results of more than one comparison operator
- ex: `((5 < 2) && (2 >= 3))`
    - the above example will check if five is less than two (false), AND(&&) if two is greater than three (false). This would resolve as true only if both comparisons resolved as true, which is not the case here.
- `&&`: the logical and tests more than one condition and returns true only if all conditions applied return true
- `||`: the logical or tests one condition at a time, and returns true if it finds any condition that returns true
- `!`: the logical not reverses the state of an expression

## Loops!
- Loops check a condition and then continue to run as many times as that condition remains true
- For loops:
    - runs a specific number of times based on a counter
    - ex: `for(var i = 0; i < 10, i++)`
    - the above loop starts at zero, and runs because 0 < 10. All the code within the loop will the run and the counter will increment by one (due to the `i++` increment command). This will continue 10 times, and once the counter reaches 10 the loop will stop running and the code moves on.
    - For loops are followed by a set of curly brackets `{}`, the opener right after the closing parenthese of the counter, and the closer at the end of the code block that the for loop executes.
- While loops
    - While loops run an infinite number of times as long as their conditional remains true
    - the variables used in a while loop should be established outside the loop, and then updated inside the loop.
    - ex:
    `var i = 1;`   *this sets i, our counter, to one*
    `var msg = '';` *the string 'msg' is currently empty, but the variable has been declared*

    `while(i<10) {` *every time i is less than 10, the loop will repeat*
      ` msg += i + ' x 5 =' + (i * 5) + <br />;` *adds on to what already existed (+=), then concatinates i (counter), the string ' x 5 =' , the result of that operation, and then includes a line break. The output of this line of code on the first run of the while loop would be: 1 x 5 = 5. The line break would then move you to the next line*
    `i++` *increases the counter by one*
    `}` *closes the loop*
- Do While loops
    - in Do While loops, the statements come before the loop starts, meaning it will always run at least once.
    - ex:
    `var i = 1;` *declaring our counter at one*
    `var msg = '';` *declaring our empty string*
    `do {` *opens the do portion of the loop*
    `  msg += i + ' x 5 = ' + (i * 5) + <br />;` *the same concatination and calculation statement as before*
    `} while (i < 1);` *closes the loop and states the run condition. The loop has already been run once, even though the counter started at one*
    
    [![Home](https://github.com/Overholtk/reading-notes/blob/master/home%20button.png?raw=true)](https://overholtk.github.io/reading-notes/)
