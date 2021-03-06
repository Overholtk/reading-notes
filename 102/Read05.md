![](https://cdn.cnn.com/cnnnext/dam/assets/150103074330-hubble-space-background-2-large-169.jpg)

# Design Web Pages with CSS

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

### Understanding Color
- Hue:
 - Corresponds to what wavelength of light is emitted
- Saturation:
 - The amount of gray in a color
- Brightness/Value:
 - Amount of black in a color
- Contrast:
 - Low Contrast: Colors are similar, makes text difficult to read
 - High Contrast: Colors are vastly different, but can cause eye strain
 - Medium contrast: Muting colors slightly allows them to fit together well for a better visual experience
- Opacity:
 - Opacity value between 0.0 and 1.0
 - RGBA allows you to set color and opacity, but is not inherited by child elements
 - To accomodate for browsers that may not allow RGBA, you can add fallback using the rules of precedence
- HSLA
 - Similar to RGBA, but subs out brightness for lightness. Lightness allows one to control both the black and white balance in a color.
 - Not always supported on old browsers, one should include a fallback for every usage of HSLA
 


[![Home](https://github.com/Overholtk/reading-notes/blob/master/home%20button.png?raw=true)](https://overholtk.github.io/reading-notes/)
