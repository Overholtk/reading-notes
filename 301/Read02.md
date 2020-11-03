# Pair Programming & jQuery

## jQuery
- "jQurty is a JavaScript file that you include in your web pages. It lets you find elements using CSS-style selectors and then do something with the leements using jQuery methods."

Find Elements using css-style selectors:
- `$('li.hot')`
- performs similarly to DOM navigation but with simpler syntax
- can store the jQuery object in a variable

Do something with the elements:
- any methods to work with
- represent common takss

Why jQuery?
- common tasks in less code
- simple selectors
- cross-browswer compatibility

Looping: if a selector returns multitple elements, you can update all of them using one method (no need for a loop!)
Chaining: can list several methods at the same time using dot notation on one selection of elements

`.html()`: retrieves the HTML of the first element, along with it's descendants

`.text()`: gets just the text from a selection. returns content from every element in the selection along with descendants

`.replaceWith()`: replaces every element in a matched set with new content

`.remove()`: removes all of the elements in a set

`.before()`: insers content before the selected element
`.after()`: inserts content after the selected element
`.prepend()`: inserts content inside selected elements after opening tag
`.append()` inserts content inside selected elements before closing tag

`.attr()`: get or set a specified attribute and it's value
`.removeAttr()`: removes a specified attribute & value

`.addClass()`: adds a new value to the existing value of the class attribute
`.removeClass()`: removes a value from the class attribute

`.each()`: performs one or omre statements on each of the items in the selection

## 6 Reasons For Pair Programming:
1. Greater efficiency
  - takes longer but produces higher quality code
  - easier to catch mistakes
  - divide up research when stuck
1. Engaged collaboration
  - more engaging and more focued
  - helps find solutions
1. Learning from fellow students
  - exposure to new techniques
  - teach each others skill sets
1. Social Skills
  - develop interpersonal skills
  - develop ability to communicate about code
1. Job Interview Readiness
  - paired programming often featured in job interviews
  - gets a sense for how the applicant fits on the team
1. Work environment readiness
  - requires less training on how to output a product as a team

