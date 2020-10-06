## Domain Modeling
- process of creating a conceptual model in code for a specific problem
- gets everyone on the same page to understand a problem
- define a constructor and initialize properties:
  - a constructor function will define the same properties over many objects
  - declares a function then holds parameters inside properties
  - objects are instantiated with the `new` keyword, then properties are initialized by calling the constructor function with the values as params
- object-oriented programming
- function prototype

## Tables
### Four key elements for creating tables

Structure:
- `<table>` creates a table
- `<tr>` indicates the start of each row with the opening tag, and the end with the closing tag
- `<td>` indicates the start of each cell in a row with the opening tag, and the end of that cell with the closing tag

Headings:
- `<th>` th stands for table heading, used the same as `<td>` but represents the heading for either a column or row
- should still use one of these tags to denote a cell even if it has no content

Spanning rows and Columns
- `colspan` attribute can be used on a `<th>` or `<td>` element to run it acrros multiple columns
- `rowspan` can be added on to a `<th>` or `<td>` element to indicate how many rows a cell should span down a table

Long Tables
- `<thead>`: headings
- `<tbody>`: body
- `<tfoot>`: footer

## Functions, Methods, and Objects
- Constructor notation: new notation and object constructor create a blank object that can be filled with content
- property values can be updated with dot notation (`hotel.name = 'Park';`) or square bracket syntax (`hotel['name'] = 'Park';`)
- `this` keyword: references the entire object used to denote and reference varialbes

Built in objects
- objects built into the browser that can be accessed and used
- Three groups:
1. Browser: creates a model of the browser tab or window
  - Window object: top most object in the Browser object, contains objects that tell you about the browser
1. Document: creates a model of the current web page
  - represents the webpage loaded into the current browser window or tab (DOM)
1. Global: group of individual objects that relate to different parts of JavaScript

