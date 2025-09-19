Week 3: CSS Foundations - Saturday Lecture Notes
================================================

Introduction to CSS
-------------------

CSS (Cascading Style Sheets) is a stylesheet language used to describe the presentation of HTML documents. It controls how elements are displayed on web pages, including layout, colors, fonts, and more.

CSS Syntax & Selectors
----------------------

### Basic CSS Syntax

css

selector {
    property: value;
    another-property: value;
}

Example:

css

h1 {
    color: blue;
    font-size: 2rem;
}

### Types of Selectors

-   Element selector: `p { }` - selects all `<p>` elements

-   Class selector: `.class-name { }` - selects elements with `class="class-name"`

-   ID selector: `#id-name { }` - selects element with `id="id-name"`

-   Universal selector: `* { }` - selects all elements

-   Attribute selector: `[type="text"] { }` - selects elements with specific attributes

-   Pseudo-classes: `a:hover { }` - selects elements in a specific state

CSS Units
---------

### Absolute Units

-   `px` (pixels) - Fixed size unit (1px = 1/96th of 1in)

### Relative Units

-   `%` - Percentage relative to parent element

-   `em` - Relative to the font-size of the element

-   `rem` - Relative to the font-size of the root element

-   `vw` - 1% of the viewport's width

-   `vh` - 1% of the viewport's height

Colors in CSS
-------------

### Color Representation Methods

-   Keyword: `red`, `blue`, `transparent`

-   HEX: `#RRGGBB` or `#RGB` - `#ff0000` (red)

-   RGB: `rgb(255, 0, 0)` - Red, Green, Blue values (0-255)

-   RGBA: `rgba(255, 0, 0, 0.5)` - RGB with alpha transparency (0-1)

-   HSL: `hsl(0, 100%, 50%)` - Hue (0-360), Saturation (0-100%), Lightness (0-100%)

-   HSLA: `hsla(0, 100%, 50%, 0.5)` - HSL with alpha transparency

### Gradients

css

.linear-gradient {
    background: linear-gradient(to right, red, blue);
}

.radial-gradient {
    background: radial-gradient(circle, red, blue);
}

Inheritance, Cascade & Specificity
----------------------------------

### Inheritance

Some CSS properties inherit values from their parent elements (e.g., `color`, `font-family`), while others don't (e.g., `border`, `margin`).

### Cascade

When multiple rules apply to the same element, CSS follows a cascade order:

1.  Importance (`!important`)

2.  Specificity

3.  Source order (later rules override earlier ones)

### Specificity

The algorithm browsers use to determine which CSS rule applies:

1.  Inline styles (1000)

2.  IDs (100)

3.  Classes, attributes, pseudo-classes (10)

4.  Elements, pseudo-elements (1)

Example: `#nav .item.active` has specificity 100 + 10 + 10 = 120

Box Model
---------

Every element is represented as a rectangular box with these components:

-   Content: The actual content of the element

-   Padding: Space between content and border

-   Border: Line around the padding

-   Margin: Space outside the border, between elements

<https://mdn.mozillademos.org/files/16558/box-model.png>

### Box-Sizing

The `box-sizing` property defines how the width and height of elements are calculated:

-   `content-box` (default): Width/height = content only

-   `border-box`: Width/height = content + padding + border

css

* {
    box-sizing: border-box; /* Recommended practice */
}

Display Types
-------------

-   Block: Elements take full width, create new line (div, p, h1-h6)

-   Inline: Elements flow in text, respect left/right margins (span, a, strong)

-   Inline-block: Like inline but respects width/height (input, button, select)

-   None: Element is completely removed from layout

Overflow
--------

Controls what happens when content overflows its container:

-   `visible` (default): Content is not clipped

-   `hidden`: Content is clipped, no scrollbars

-   `scroll`: Always show scrollbars

-   `auto`: Show scrollbars only when needed

Best Practices
--------------

-   Use external stylesheets for maintainability

-   Use semantic class names that describe purpose, not appearance

-   Organize CSS with comments and logical grouping

-   Use relative units (rem, em, %) for responsive design

-   Always include fallbacks for newer CSS properties

-   Use the border-box model for predictable sizing

-   Validate your CSS with tools like the W3C CSS Validator

Resources
---------

-   [MDN CSS Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)

-   [CSS Tricks Guide](https://css-tricks.com/guides/)

-   [W3Schools CSS Tutorial](https://www.w3schools.com/css/)

-   [Can I Use](https://caniuse.com/) - Browser compatibility tables