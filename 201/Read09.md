## Forms

**Form Controls:**
- Adding text
- Making choices
- Submitting forms
- Uploading Flies

**Form Structure:**
- `<form>` creates the form element
- `action` attribute determines where the information will go after the user inputs it
- `method` defines the *way* a form will be sent, either with get or post
  - get: good for short forms, adds the value to the end of a url (good for searches)
  - post: long, allows for file upload, updates a database
- `<input>` element creates form controls:
  - `type='text'`
  - `name`
  - `maxlength`
  - `size`
  - `type ="password"`
- `<textarea>` defines a multi line input
- radio buttons allow users to pick one option from a given list
- checkbox allows a user to pick multiple options from a given list
- drop down list allows a user to select from a drop down
- select is similar to drop down but allows for multiple choices
- file input lets a user input a file
- submit button sends the form

## Lists, tables, and forms
- Bullet point styles
- un ordered or ordered
- disc, circle, square
- decimal, decimal leading zero, lower-alpha, upper-alpha, lower-roman, upper-roman
- bullet points can be decimals


## Events
- any kind of event can be used to trigger a function
- select the elements you want the script to respond to, indicate which event will trigger a response, state the code to be run
- DOM event handlers are recognized by all browsers but can only be attached to one function
- Event Listeners: not supported in older browsers but can deal with multiple functions
- Event flow: only really matters when code has event handlers on an element and one of it's ancestor or descendent elements, basically the string of events following an `event`
