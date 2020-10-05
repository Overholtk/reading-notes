## Objects
**Objects** group together a set of variables and fucntions
- property: a variable that is part of an object
- method: a function inside of an object
- key: the assigned name of a property or method
  - cannot have two keys with the same name (similar to IDs)
  
Literal Notation:
`var hotel ={`  <- hotel object is sotred as a variable
 `name: 'Quay',`
 `rooms: 40,    <- properties
 `booked: 25,`
 `checkAvailibility: function() {` <- method
 `return this.rooms - this.booked;`
 `}`
 
 - dot notation: to access a property or method of an object you use the name of the object, followed by a period, then the name of the property or method
  - the period is known as a member operator
- square bracket syntax: same deal but use brackets instead of a period

## Document Object Model

DOM tree:
- stored in the browsers memory and consists of four types of nodes:
1. Document Node: represents the entire page & is correlated to the document object. Navigates to all other nodes
1. Element Node: describes the structure of the HTML page
1. Attribute Node: accesses the attribute of the element you are looking at
1. Text node: reaches the text of an element
- Working with the DOM tree: access elements then work with those elements
- DOM queries: methods that find elements in the DOM tree
- When a DOM method can return more than one element it returns a NodeList
  - look and are numbered like an array but are called a collection
- whitespace is usually treated as a text node and can make a page take longer to load
  - remove whitespace
  - or use a JS library

XSS attacks:
- untrusted data: data you do not have complete control over
- validation: only allow users to input the kind of characters they need
- double check validation before displaying or storing
- Do not place users content in: script tags, HTML comments, tag names, attributes, or css values
- Escaping user content: any user inputs that contain characters that are used in code should be escaped on the server
