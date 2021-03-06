![](https://cdn.cnn.com/cnnnext/dam/assets/150103074330-hubble-space-background-2-large-169.jpg)


## Text in HTML

### Headings and Paragraphs

**Headings**
- HTML has 6 headings in various sizes, starting from the biggest with h1 and shrinking down to h6.
- Headings are denoted with a `<h#>` tag where the pound sign is replaced with the number corresponding to the chosen heading size.

**Paragraphs**
- each paragraph is surrounded by an opening `<p>` tag and a closing `</p>` tag
- by default there will be space between any two given paragraphs

### Bold, italics, and emphasis

**Bolded** statements are enclosed in a `<b>` tag that opens and closes in the same fashion as the `<p>` tag.

*Italicized* statements use the tag `<i>`
  
**Sub and superscript**
- the tag for super script is `<sup>` and the tag for subscript is `<sub>`

### Structural and semantic markup

**Structural markup** consists of the elements that can be used to describe both headings and paragraphs.

**Semantic markup** provides extra information such as emphasis, etc.
- the `<strong>` element denotes important elements that will be automatically bolded
- the `<em>` element indicates subtle emphasis and will automatically italicize when applied
- quotations can be marked up using the `<blockquote>` tag or `<q>` tag. 
  - blockquote is for longer, paragraph length quotes
  - q is for shorter, phrase length quotes
- `<abbr>` denotes an acronym
- `<cite>` marks a piece of information as a citation, `<dfn>` marks as a definition
- `<address>` should contain the author's information and will often be displayed in italics
- `<ins>` and `<del>` shows what content has been inserted or deleted. ins will usually underline content, del will strikethrough
- `<s>` denotes outdated or irrelevent information that shouldn't be deleted and will strikethrough
  

### Misc. Info

HTML is not **white space** sensitive, so code authors can choose to leave blank spaces to improve readability without sacrificing functionality.

**Line breaks** will add a break inside of a single paragraph, and uses the tag `<br />`

**Horizontal rules** create a visual line that can seperate two subjects, and are created with the `<hr />` tag

## Intro to CSS
## CSS

allows you to create rules that specify how the content of an element should appear.

### How does it work?
CSS associates rules with HTML elements
Two parts of a rule:
1. Selector: indicates what the rule applies to
 1. Declaration: indicates styling for said elements
      - Declaration Property: indicates what is being styled (font, color, etc.)
      - Declaration Values: indicates what it is being styled to (Arial, yellow, etc.)

Ex: `{`
    `font-family: Arial;`
    `color: yellow}`

### External CSS
The **link** element is used to link an HTML file with it's corresponding CSS document.

**href** specifies the path to the CSS file

**type** specifies what kind of document is being linked (CSS or text)

**rel** specifies how the document is related to the HTML page. When using the "CSS" type, this value should always be "stylesheet"

Combining all these elements to properly link a CSS document will look like this:

`<link href="path to document" type="text/css" rel="stylesheet" />`

If using more than one CSS stylesheet, a link element would be required for each

### Internal CSS
CSS can be used directly on top of HTML coding, without the need for a second page. 

The **style** element denotes an area where we are coding in CSS, and is usually found in the `<head>` of the file.

Internal CSS should not be used on a site with more than one page.

### CSS selectors

Selectors allow you to target specific aspects of HTML to change, they are case sensitive. Below are some of the most common ones.

Selector     |    Meaning    | Example     
-------------|---------------|--------------
Universal| Applies to all elements | `* {}` |
Type | Matches element names | `h1, h2, h3 {}` |
Class | Matches to class attribute | `.note {}` |
ID | Matches to ID attribute | `#introduction {}` |
Child | Matches an element that is a direct child of another | `li> {}` |
Descendant | Matches an element that is a descendant of a specified element | `p a {}` |
Adjacent Sibling | Matches an element thats the next sibling of another | `h1+p {}` |
General Sibling | Matches an element that is a sibling of another | `h~p {}` |

### CSS Rules Precedence

**Last Rule:** If the two selectors are identical, the latter of the two will take presedence

**Specificity:** If one selector is more specific, it will take presedence.

**Important:** Add `!important` after any property value to flag it as more important than others

### Inheritance

Many properties are **inherited** by most child elements (ex: body to section), such as font style and color. If a property is not inherited and you would like it to be, you can use `inherit` for the value property of that element.

## Color
The **color property** allows for specifying the color of text inside an element.

3 ways to Specify Color:
- RGB values:
 - numerical values of the amount of red green and blue.
- Hex Codes:
 - Six digit codes representing rgb numbers
- Color Names:
 - Using predefined color names

Every computer screen is made up of pixels that are able to emit light and create images.

## Basic Javascript

### Statements
- each step in a script is a statement
- should end with a semicolon
- case sensitive
- code blocks are surrounded by curly brackets

### Comments
- explain what your code does
- can be multi or single line

### Variables
- a place to store bits of information
- must be declared and then assigned a value
- Data types:
  - numeric
  - string
  - boolean

### Arrays

- a variable that stores a list of values
- initialize like any other variable and then assign a list of values seperated by commas
- first term is 0

## Decisions and Loops

## Decisions
- allows code to take one path or another
- often uses booleans
- sets a condition to evaluate against
- uses logical operators, if statements, and if/else statements

[![Home](https://github.com/Overholtk/reading-notes/blob/master/home%20button.png?raw=true)](https://overholtk.github.io/reading-notes/)
