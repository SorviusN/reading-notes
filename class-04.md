
# Topics for HTML/CSS Book:
  - Links (74 - 93).
    - Directory Structure
    - Relative URLs
  - Layouts (358 - 404).
    - Normal Flow
    - Relative Positioning
    - Absolute Positioning
    - Fixed Positioning
    - Floating Elements

## Links
- Defining feature of the web, focuses on linking one website to the next.
- Linking to other sites:
``` Javascript
<a href="Link content">Click this to access the content.</a>
```
- You may also link to sites on same page. This can be done as such:
``` Javascript
<a href="movies.html">Movies</a>
<a href="contact.html">Movies</a>
```
### Directory Structure.
- Always place html, css and JS files in their respective folders.
- Root folders are main folders.
- Use URLs when linking to other web pages and when including images on your own site. They should have their own respective folders.

### Relative URLs
- ALL BELOW SHOULD BE RELATIVE TO HTML
- Same Folder 
- Child Folder
- Grandchild Folder
- Parent Folder
- Grandparent Folder

### Email Links
``` Javascript
<a href="mailto:jona@berklee.edu"> </a>
```
- To open links in new window, use "target=blank"

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
### Positioning of elements
- Normal: every block-level element appears on a new line.
- Relative positioning: Moves element from position it would normally be in 
- Absolute positioning: positions element in relation to its containing element. Is taken out of normal flow.
- Fixed positoning: form of absolute positioning that positions the element in relation to the browser window.
- Float Elements: Allows element to be out of flow and position to far left/right  of containing box. 
IMPORTANT: Floated element becomes a box-level element which other content can flow.

# Topics for JS/JQuery:
 - Functions, Methods and Objects (86-99) 
  -Functions
  -Objects

## Functions
- Lets you group a series of statements together to perform a specific task. Can call arguments as well.
- They can be executed whenever certain conditions are met either on a webpage or in a program/script.
``` Javscript
function doSomething() {
  var thing = 'This is a string'
  alert(thing);
  }
```
- You may also use functions that return values, such as true, int or string.
- Arguments can be passed into functions that perform actions with the data.

## Objects
- What is an object? - They group together a set of variables and functions to model a thing that you would recognize in real life.
- Functions are known as methods inside of objects.
``` Javascript
var Painting {
//variables
  name: 'The Scream',
  width: 1,
  value: 29.6,
  isFamous: true,
//Methods
isFamous: function() {
  return this.isFamous }
  };


