## Layout
- Containing Elements: if a box level element is inside another box level element, the outer element is considered the containing or parent element
- Types of positioning:
  - Normal: block level on new line
  - Relative: shifts the position of that specific element up down left or right
  - Fixed: positions element in relation to the browser window
  - Floating: takes an element out of the normal flow and positions it to the far left or far right of its containing element
- Z-index: controls which element sits on top when two elements overlap, sometimes refered to as the stacking context
- Clearing floats: clear property allows you to say no element within the same containing element should touch the left or right-hand sides of a box

**Fixed Width Layouts:**

Advantages:
- pixel values are accurate at controlling size and positioning of elements
- greater control over appearance, position of items
- control the lengths of lines of text
- image size remains the same relative to the rest of a page

Disadvantages:
- Gaps around the end of a page
- Resolution of the user's screen can affect readability
- If use changes font sizes they might not fit
- works best on devices that have a resolution similar to laptops or desktop computers
- take up more vertical space than a liquid layout

**Liquid Layouts**

Advantages:
- Pagees expand to fill the entire browser
- Contract to fit small window size
- Tolerant of users altering fonts

Disadvantages:
- Section width can cause gaps or squishing elements together
- Lines of text can be very long if the user has a wide window
- narrow windows can cause text to be squished
- if a fixed width item is too small for it's container it can spill over into the other elements of the page

**Layout Grids**
- set consisten proportions and spaces between items
- helps users predict where to find information
- makes it easier to add new content 
- helps people stay on the same page visually
