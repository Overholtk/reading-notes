# Flexbox and Templating

## Mustache.js
Templating: efficient way to render client-side view templates with JS by using JSON. Added tags either insert variables or run logic.

Mustache: logic-less template syntax
- can be used for HTML, config files, source code, etc.
- no if, else, or loops. only tags.
- mustache.js is an implementation of the mustache template
- `{{name}}` double brackets denotes a placeholder
- not a templating engine
- mustache-express: uses mustache and express together easily

## Flexbox:
Properties for the parent container:
- display: flex
- flex direction: establishes the main-axis and defines the direction flex items are placed in the container
  - row, row-reverse, coloumn, column-reverse
- flex-flow: shorthand for flex-direction and flex-wrap properties
- justify-content: defines the alignment along the main axis. helps distribute extra free space
  - flex-start
  - flex-end
  - start
  - end
  - left
  - right
  - center
  - space-between
  - space-around
  - space-evenly
- align-items: defines the default behavior fow how flex items are laid out along the cross axis on the current line
  - stretch
  - flex-start/ start/ self-start
  - flex-end/ end/ self-end
  - center
  - baseline
- align-content: aligns a flex containers lines within when there is extra space on the cross axis (only takes effect on multi-line containers)
  - normal
  - flex-start
  - flex-end
  - center
  - space-between
  - space-around
  - space-evenly
  - stretch
  
Properties for flex items (children):
- order: controls the order in which the items appear in the flex container (default laid out in source order)
- flex-grow: defines the ability for an item to grow, accepts a unitless value that dictates how much of the availible space it should take up
  - positive numbers only
- flex-shrink: defines the ability for a flex item to shrink if necessary (no negatives)
- flex-basis: defines the default size of an element before the remaining space is distributed 
  - auto: "look at height and width property"
  - 0: the extra space is ignored
- flex: shorthand for flex-grow, flex-shrink, and flex-basis
- align-self: allows the default alignment to be overridden for individual flex items
