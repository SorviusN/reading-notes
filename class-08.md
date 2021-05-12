# Topics for Class 8
- Layouts



## Layouts
- Building Blocks, block level element starts on a new line. such as h1, p, and footer
- Inline elements flow in between surrounding text, such as img, b, and i.
- If one block level element sits inside another, the out box is the parent:

``` Javascript
<header class="Parent">
  <h1 class="Child"></h1>
  <img href="something" class="Child">
</header>
```
### Normal Flow
- Every block-level element appears on new line, causing each item to appear lower down the page.
### Relative Positioning
- Moves element from position it would be in flow, shifting to the top, right, bottom or left of where it would be placed. Does not affect position of surrounding elements.
### Absolute Positioning
- Positions element relative to its containing element.
### Fixed Positioning
- Form of absolute positing that puts element in relation to browser window. Does not move when scrolling.
### Floating Elements
- Float allows to take element out of normal flow and position to far left or right of a containing box. 
- It becomes a block level element around which other content flows.

### Overlapping Elements
- use z-index property to determine hierarchy with what element is on top of others when overlapping.

### Types of Layouts
- Fixed layout: width of main boxes on a page will be specified with pixels 
- Liquid layout: uses percentages to specify the width of each box so that the design will stretch to fit size of screen.
- Grid layout: Content is made up of different grids, where everything is positioned on a grid x and y axis.

