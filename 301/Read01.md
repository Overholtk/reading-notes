# SMACCS and Responsive Web Design

## Responsive Web Design:
- RWD: "...the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop."

### Responsive vs. Adaptive vs. Mobile
- Responsive: react quickly and positively to any change.
  - change based on size of viewport
- Adaptive: easily modified for a new purpose or situation.
  - built to a group of pre set factors
- Mobile: build a separate website solely for mobile users.
  - occasionally has it's place but not usually a good idea

### Flexible Layouts
- building the layout of a website on an easily resizable grid
- doesn't used fixed measurement like pixels
- `target width of element / width of parent element = width of target element`
- viewports can become too small to use flexible layouts
### Media Queries
- provide the ability to specify differnt styles for different circumstances
- `@media` rule, `@import` rule, and linking to a separate stylesheet

### Mobile First:
- define the mobile style first then add more as the viewport grows
- avoids a mobile user having to load the desktop styles and then have them written over
- design with a mobile user in mind

### Flexible Media:
- making images, videos, etc. scalable
- `max-width` property at 100%
- embedded media work around: absolutely positioned inside a parent element

## Floats:
- float elements remain a part of the flow of a web page
- valid values: left, right, none, inherit
- clearing the float: `clear` property moves an element below the floated element
  - 4 valid values: both, left, right, none
- a parent element containing only floated elements can collapse
