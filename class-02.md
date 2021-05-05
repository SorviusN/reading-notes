# Reading 02 Notes

## Topics for HTML/CSS Book:
* Structural Markup/Semantic Markup
* Headings/Paragraphs
* Abbreviations/Acronyms, Citations/Definitions
* Strong & Emphasis/Quotations  

## Topics for JS/JQuery Book:
* Language Syntax & Grammar
* Code Blocks and Variables
* Data Types
* Rules for naming variables
* Arrays
* If else and while statements

### Simple webpage that demonstrates text Markup:

``` HTML5 
<html>
  <head>
    <title>Text</title>
    <link href="myLink"/>
  </head>
  <body>
    <h1> </h1>
    <h2></h2>
    <p>This is information for a <i>paragraph</i>. It can contain a lot at times. </p>
  </body>
</html>
```

### Structural/Semantic Markup
  - Structural is for elements that you can use to describe both headings and paragraphs.
  - Semantic provides more info - one example being bold or quotation marks.

### Headings and paragraphs
  - There are 6 levels of headings, h1-h6. h1 is largest.
  - By default, a browser will show each paragraph on a new line with some space between it and any other paragraphs.
  - It is good practice to split up paragraphs into smaller forms of text.

### Abb/Acronymns and Citations/Definitions.
  - Abbreviations give the user extra information on when hovering over. Example could be cont. for continuted. <abbr></abbr>
  - Acronyms work similarly, except hover over the entire name of the acronym. Example could be NASA, for National Aeronautics and Space Administration <acronym></acronym>

### Strong and Emphasis quotations 
  - the elements <b></b> and <em></em> are used frequently to add dynamic expression to your markup. Very common in articles.

### Code Blocks and Variables
 - Variables are what we store data types inside of. We are essentially telling the computer a specific name for a type of data (or lack of data) in memory.
 - A variable can change data types as well after creating.
 - Code blocks are used to separate code into neater sections. Some code blocks can act as "gates" that will only be run of certain conditions are met or a function is called.

### Data Types
 ``` Javascript 
// Numeric Data Type -
let num = 0.75
// String Data Type - 
let hello = 'Hi there.'
// Boolean type
let onOrOff = true
```

### Naming Variable Rules - quoted from Jon Duckett Javascript & JQuery, Page 69
  - Must begin with a letter, dollar sign or underscore.
  - can contain letters, numbers, dollar sign or an underscore. Cannot use dash or period in var name.
  - Cannot use reserved keywords.
  - All variables are case sensitive. score and Score would be different.
  - Use a name that describes the kind of information that the variable stores.
  - If your variable is made up of more than one word, use a capital letter for the first letter of every word after first word (camel case).

### Arrays
``` Javascript
//Creating an array -
var drinks;
drinks = ['water',
'juice',
'soda',
'beer'];

drinks[0] === 'beer';
```
### If else and While statements
  - There are two components to the decision in If else.
  - In the while loop, the action in the code block will continue to be performed until the condition is met from the while loop.
