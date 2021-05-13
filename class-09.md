# Reading notes for Class 9 

# Topics for HTML/CSS:
- Forms (144 - 175)
- Lists and Tables (330 - 357)

## Forms

### Summary
- whenever you want to collect info from visitors you will require form.
- lives inside of the form element
``` html
<form></form>
```
- info  from form is sent in name/value pairs
- mainly used for collecting data from user and doing something with that data.

### Form Controls
- Adding text
  - Text input
  - password input
  - text area (for longer areas)
- Making choices
  - Radio buttons
  - checkboxes
  - Drop-down boxes
- Submitting forms
  - Submit button
  - Image buttons
  - Uploading files (upload button)

### How they work
- Use form text to fill out, and a button to submit.
- Server needs to know which piece of inputted data corresponds with the right element.

### Types
- type="password" can also carry size and maxlength variables.


## Lists and tables
- Bullet point styles
- adding borders/backgrounds to tables
- changing appearance of form elements.

### Bullet point styles
- Created with list-style-type
- Unordered lists
- Ordered lists
- can also use images for bullets with list-style-image
- list-style-position can indent the marker to be isnide of the text.
- list-style serves as a tool for adjusting image, style and position property in any order.
``` css
ul {
  list-style: inside circle;
  width: 300px;
  }
li {
  margin: 10px 0px 0px 0px;
}
```

### Table properties
- width to set width of table
- padding to set space between border and each table cell/content
- text-transform, converts the content of the table headers to uppercase 

### Empty cells/gaps between cells
- the "show" property shows the borders of any empty cells
- "hide" hides borders of empty cells
- inherit instructs table to obey rules of containing cells

### Collapse 
- border-spacing gives margins between the borders of the tables
- border collapse: collapse into single border where possible
- border collapse: separate gives them all different squares

### Cursor Styles
- auto
- crosshair
- default
- pointer
- move
- text
- wait
- help
- url ("cursor.gif")

## Topics for JS 
- Events (243 - 292)

## Events

### What are they?
- Scripts respond to events by the user, which makes page feel more interactive.
- Interactions create events, events trigger code and code responds to users.

### Different event types
UI EVENTS
  - load
  - unload
  - error (something went wrong)
  - resize (size up or down with page)
  - scroll (scrolling up or down page)

- KEYBOARD EVENTS
  - keydown
  - keyup
  - keypress

- MOUSE EVENTS
  - click
  -dblclick
  - mousedown
  - mouseup
  - mousemove
  - mouseover
  - mouseout
- FOCUS EVENTS
   - focus
   - blur
- FORM EVENTS
  - input
  - change
  - submit
  - reset
  - cut
  - copy
  - paste 
  - select

### Steps to trigger an event in JS code
1. select the element that you want your script to respond to
2. indicate which event on the selected nodes will trigger response (called "binding")
3. Indicate what code you want to run with hte event, may be named or anonymous

### Traditional DOM event handlers
``` js
functionName() {
  do something
}
element.onevent = functionName // make sure to not put parentheses.
```

### Event listeners
``` js
element.addEventListener('event', functionName [, Boolean]) // last value indicates something called capture, usually set to false.
```
