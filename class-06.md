# Class 06 reading notes

# Topics for JS:
- Object Literals (100- 105)
- Document Object Model (183-242)

## Object Literals

### What are objects?
- Objects are a set of functions and variables grouped together to form something that we would recognize in the real world.
- Objects and functions = Properties and Methods when talking about an object.
- Properties and methods have a name and value. The name is the key.

``` js
var computer = {
  name: "My Computer",
  isOn: true;
  processingPower: 1000,

  checkIfIsOn: function() {
    return this.isOn;
    }
  }
```

### Literal notation/ Accessing an object and dot notation
- Literal notation is most popular way to create objects. It is shown above.
- You can access properties and methods using dot notation.
- When referencing an object property or function, you may use computer.name as an example.

### Referencing objects with getElementById
- you may reference javascript variables with HTML. Example could be:

``` js
//modeled after a hotel. The top portion represents giving elName the rooms element in HTML. 
// The bottom portion is giving elName the value of whatever the hotel object name is.

var elName = document.getElementById('hotelName');
elName.textContent = hotel.name();
```


## Document Object Model
- Specifies how browsers should create a model of an HTML page + how Javascript can access/update contents of web page in browser.
- The DOM defines methods and properties to access and update each object in the model.

### Four main types of nodes
- Document node: the HTML of the page is the bones of the project. Contains all text information inside of it.
- Element nodes: Elements describe the structure of HTML (like h1, p, div). To access DOM tree, you start by looking for elements. You can access element nodes with JS and CSS.
- Attribute nodes: opening tags of HTML can carry attributes, represented by attribute nodes. they are not children, but are actually part of the element. (Example is: class="large-content")
- Text nodes: After accessing an element node, you can reach text within the element - stored inside of its own text node. Text node cannot have children nodes, the corresponding element node does.

### Working with the DOM tree.
- Access the elements.
``` js
Document.getElementById('thisId'); // Uses value of an element's ID attribute.
Document.querySelector('.myClass'); // Uses CSS selector and returns first matching elements.
```
 - Select Multiple Elements (Nodelists)
 ``` js
//Three common ways to select multiple elements.
Document.getElementByClassName('.myClass');
Document.getElementsByTagName(li);
Document.querySelector();
 ```
### Looping through a NodeList
- When you have a nodelist, you can loop through each node in collection and apply same statements to each.

``` js
var greenItems = document.querySelectorAll('div.green');
for (let i = 0; i < greenItems.length; i++) {
  greenItems[i].className = 'red'} //changing the class of the divs in question from green to red.
```

### Traversing the DOM
- parentNode finds the element node for the containing(parent) element in HTML.
- previousSibling, nextSibling.
- firstChild, lastChild.
- Most browsers, except IE, treat whitespace between elements (spaces) as a text node, so properties above can return different elements in different browsers.
- A solution to this is to use JQuery.

### Accessing and updating text with TextContent
``` js
var firstItem = document.getElementById('one').textContent;
firstItem.textContent = 'bread'; // updates the inner text 
``` 
### Removing elements form the DOM Tree

``` js
var removeElement = document.getElementByTagNae('li'[2]); // The element to remove

var parentElement = removeElement.parentNode; // Its containing element

parentElement.removeChild(removeElement); // Removing the element
```
