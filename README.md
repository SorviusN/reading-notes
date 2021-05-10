# Code 201 Reading Notes
Reading notes file for Code Fellows.
Table of Contents for 15 Daily Assignments -
1
2
# CLASS 3 - 
#Lecture Notes

## False Value in Javascript
  - false
  - 0  (zero)
  - ' ' (empty string)
  - null
  - undefined
  - Nan (not a number)

``` javascript
if (somethingEvaluatesTrue) {
  then perform an action
  }
```
## comparison operators
  a == b - "loosely equal to" 10 == '10' - type coercion / weak typing.
  weak typing ^

  a === b - "strictly equal" to 10 === 10
  a !== b - "not equwal to (! called bang!) 10 !== '10'"
  a != b - "not loosely equal to 10 != 'banana'"
  a > b - a is greater than b
  a < b - a is less than b
  a >= b - greater than or equal to

## logical operators

&& - and a && b - both HAVE to be true.

## Arrays
  - datatype of Object.
  - a list of elements - the elements within the array can be dt
  - ['car', 1, {name: 'Sara'}] try not to have arrays with mixed elements.

## Why?
- saves us from needing to repeat code.

# Class 4 Lecture Notes

# Display and Position
- two properties that will help wontribute to you getting your layout to look the way you want it to.

## display: inline
- puts alament inline with other elements around it. Any height and width properties will have no effect.

## display: inline-block
- Compared to display: inline, the major difference is that display; inline-block allows to set a width and height on the element.

- Also, with inline block, the top and bottom margin/paddings are respected, but with display: inLine they are not.

## display: block
- Displays an element as a block element (like p), 

### Position Absolute
Essentially does the same thing as position: relative with two key differences:
The element is taken out of normal flow and leaves no space behind.
The element is positioned relative to its nearest parent with a relative-type (relative, absolute, fixed)

### Position Fixed

Fixed is the same as absolute with one key difference:
The element is positioned relative to the browser/viewport.


## Functions

### what 
- a function is a group of statements that perform a task or calculate a value. Stored within  a structure that prevents them 
from running until function is called or invoked.

### why
- functions are reusable.
- functions make our code DRY
- Prevents bugs

``` javascript
function bakeCake() {
pour ingredients into bowl
mix ingredients
pour batter into pan
bake for 40 mins at 350
}
```


# Lecture Notes for Class 5 

## css

### designing a webpage
- create an idea of the layout before you write the HTML
- identify the parts you need first
- write html to fit your design, not other way around.

## git branches

### 
# Lecture Notes 6

## const

### what?

- a way to declare variables whose vlaue will never change
- a constant valued varible

### why?
- it never can be changed, prevents code errors and tells better story.
``` js
const newVariable = 'unchanging';
```

## template literals

- a new way to write string without concatonation
- wrap string in backticks.

``` js
let thing = `This is a string with the variable ${newVar} inside of it.`
```

## Custom google fonts



#7
#8
#9
#10
#11
#12
#13
#14
#15

