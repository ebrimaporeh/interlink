Week 3: CSS Layout & Positioning - Sunday Lecture Notes

=======================================================

Positioning

-----------

CSS positioning allows you to control the placement of elements on a web page.

### Position Values

-   Static (default): Elements flow in normal document order

-   Relative: Positioned relative to its normal position

-   Absolute: Positioned relative to nearest positioned ancestor

-   Fixed: Positioned relative to viewport (stays on screen during scroll)

-   Sticky: Hybrid of relative and fixed positioning

css

.relative {

    position: relative;

    top: 20px;

    left: 30px;

}

.absolute {

    position: absolute;

    top: 0;

    right: 0;

}

.fixed {

    position: fixed;

    bottom: 20px;

    right: 20px;

}

.sticky {

    position: sticky;

    top: 0;

}

### z-index & Stacking Context

The `z-index` property controls the stacking order of positioned elements. Higher values appear in front of lower values.

css

.element {

    z-index: 10; /* Appears above elements with lower z-index */

}

A stacking context is formed when:

-   Element is the root element (HTML)

-   Element has position other than static and a z-index value

-   Element has opacity less than 1

-   Element has certain transform, filter, or perspective properties

Float & Clear (Legacy Layout)

-----------------------------

Floats were originally for text wrapping around images but were used for layouts before Flexbox/Grid.

css

.float-left {

    float: left;

    margin-right: 15px;

}

.float-right {

    float: right;

    margin-left: 15px;

}

.clearfix::after {

    content: "";

    display: table;

    clear: both;

}

Flexbox

-------

Flexbox is a one-dimensional layout model for arranging items in rows or columns.

### Flex Container Properties

css

.flex-container {

    display: flex; /* or inline-flex */

    flex-direction: row; /* row, row-reverse, column, column-reverse */

    justify-content: flex-start; /* flex-start, flex-end, center, space-between, space-around, space-evenly */

    align-items: stretch; /* stretch, flex-start, flex-end, center, baseline */

    flex-wrap: nowrap; /* nowrap, wrap, wrap-reverse */

    align-content: stretch; /* Similar to justify-content but for cross-axis */

}

### Flex Item Properties

css

.flex-item {

    flex-grow: 0; /* How much item grows relative to others */

    flex-shrink: 1; /* How much item shrinks relative to others */

    flex-basis: auto; /* Default size before growing/shrinking */

    flex: 0 1 auto; /* Shorthand for grow, shrink, basis */

    order: 0; /* Visual order (doesn't affect source order) */

    align-self: auto; /* Overrides align-items for individual item */

}

### CSS Grid

--------

CSS Grid is a two-dimensional layout system for the web.

### Grid Container Properties

css

.grid-container {

    display: grid; /* or inline-grid */

    grid-template-columns: 100px 1fr 2fr; /* Column sizes */

    grid-template-rows: 100px auto; /* Row sizes */

    gap: 10px; /* Shorthand for row-gap and column-gap */

    row-gap: 10px;

    column-gap: 15px;

    grid-template-areas:

        "header header header"

        "sidebar content content"

        "footer footer footer";

    justify-items: stretch; /* Align items along row axis */

    align-items: stretch; /* Align items along column axis */

    justify-content: start; /* Align grid along row axis */

    align-content: start; /* Align grid along column axis */

}

### Grid Item Properties

css

.grid-item {

    grid-column: 1 / 3; /* Start at line 1, end at line 3 */

    grid-row: 1 / 2; /* Start at line 1, end at line 2 */

    grid-area: header; /* Reference to grid-template-areas */

    justify-self: stretch; /* Align individual item along row axis */

    align-self: stretch; /* Align individual item along column axis */

}

### Advanced Grid Features

css

.grid-container {

    /* Responsive columns */

    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));

    /* Using minmax() for flexible sizing */

    grid-template-columns: 1fr minmax(300px, 2fr) 1fr;

    /* Using auto-fill vs auto-fit */

    grid-template-columns: repeat(auto-fill, minmax(100px, 1fr));

    grid-template-columns: repeat(auto-fit, minmax(100px, 1fr));

}

### Subgrid

Subgrid allows grid items to inherit the grid tracks of their parent.

css

.grid-container {

    display: grid;

    grid-template-columns: 1fr 2fr 1fr;

}

.grid-item {

    display: grid;

    grid-template-columns: subgrid; /* Inherits parent's columns */

    grid-column: 1 / 4; /* Span all columns */

}

Layout Best Practices

---------------------

1\.  Use Flexbox for one-dimensional layouts (rows OR columns)

2\.  Use Grid for two-dimensional layouts (rows AND columns)

3\.  Use modern layout techniques (Flexbox/Grid) over floats for page structure

4\.  Consider using CSS frameworks for complex layouts (but understand the underlying CSS)

5\.  Test layouts on multiple screen sizes and devices

6\.  Use semantic HTML to provide structure for your layouts

7\.  Consider accessibility when creating layouts (tab order, screen readers)

Responsive Design Considerations

--------------------------------

1\.  Use relative units (%, rem, em, vw, vh) for flexible layouts

2\.  Implement media queries for breakpoints

3\.  Test on various device sizes

4\.  Consider mobile-first design approach

5\.  Use flex-wrap and grid auto-placement for responsive layouts

Browser Support

---------------

-   Flexbox: Well supported in all modern browsers

-   CSS Grid: Well supported in all modern browsers

-   Subgrid: Limited support (check current status on [caniuse.com](https://caniuse.com/))

-   Always provide fallbacks for older browsers when using newer features

Resources

---------

-   [CSS Tricks Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

-   [CSS Tricks Complete Guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)

-   [MDN CSS Layout](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout)

-   [Grid by Example](https://gridbyexample.com/)