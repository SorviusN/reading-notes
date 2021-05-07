# Reading Notes - Class 3

# Topics for HTML/CSS Book:
  - Numbered Lists
  - Boxes

## Lists
- There are ordered lists, unordered lists and definition lists.
- Browsers indent lists by default.
- Sometimes you may see type attribute used with the ul element to specify the bullet point (circles, squares, diamonds.)
``` Javascript
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
  <li>Item 4</li>
</ul>
```
- Definition lists are used to define terminology.
- Lists can be nested inside of each other.

## Boxes 
- Treats elements of each HTML as if it lives in its own box.
- Box dimensions are width and height
- Most popular way to specify size of box is using pixels, percentages or ems (rems).
- Min-Width and Max-Width exist to set boundaries for how large or small a box should be.

### Overflow Content
- Tells the browser what to do if the content contained with a box is larger than the box itself.
- Hidden just hides the extra content obviously.
- Scroll adds scrollbar so that users can see missing content below.

### Border, Margin, Padding
- CSS treats each HTML element as if it's its own box.
- Border deals with the actual border of the box in question.
- Margin focuses on the space between the parent container and the actual content.
- Padding focuses on the space between the inner text elements and the box size. Larger padding = larger space between the two.


## Topics for JS/JQuery:
- Decisions and Loops" (162-182)
  - If/Else statements
  - Switch statements
  - Type Coersion
  - Loops

### If/Else statements
- Allows you to provide two sets of code - one that evaluates true and one false.
``` Javscript
if (numOfPlants >= 10) {
  performAFuntion();
  }
else  { 
  anotherFunction();
  }
```
- statements inside of an if statement should be followed by semicolon, but no need to place after closing curly braces.

### Switch statements
- Switch statement starts with value called "switch"
``` Javascript
switch(value) {
  case '1':
    value = 'something';
    break;
  case '1':
    value = 'something';
    break;
  case '1':
    value = 'something';
    break;
  default:
    'do this when the case does not have any of the above values'
    break;
    }
```
- benefits of switch case is the default statement, as well as a large amount of options to choose from with the case value.

### Type Coersion
- Every value in javascript may be treated as "truthy" or "falsey" depending on what happens to the value.
- JS is said to use "weak typing" because the data value of a variable can change at whim, based on our r value.
- Can use truthy and falsey to check if something exists or not:
``` Javascript
if (document.getElementById('section-in-html')) {
  // Found, therefore do something} 
else {
  // not found, do something else
  }
```

### Loops
-initialization, condition and update are the three parts of a loop counter.
``` 
for (int i = 0; i < 20; i++){
  thisValue += 1; // thisValue will have a value of 20 by the time the loop exits.
  }
```
