# Class 07 reading note 

# Topics:
- Domain Modeling
- Tables (HTML, 126-145)
- Functions, Methods and Objects (106 - 144)

## Domain Modeling

- Process of creating a conceputal model in code for specific problem at hand.
- entity that stores data in properties and behaviors in methods is referred to as Object-Oriented.
- We create models for our objects to determine what properties and methods they should use.

``` js
var park = funciton(hasTrees, hasAPlayground) {
  this.hasTrees = hasTrees;
  this.hasAPlayground = hasAPlayground;
  }

var ravennaPark = new park(true, false);
var lakesidePark = new park(false, false);

console.log(ravennaPark);
console.log(lakesidePark);
```
### Tips to follow when building domain models
 - When modeling single entity that will have many instsances, build self-contained objects with same att / behaviors
 - Model its attributes with a constructor function that defines and initializes properties.
 - Model its behavior with small methods that focus on doing one job
 - Create instances with new keyword follow by a call to construtor function.
 - Use the this variable within methods so you can access the object's properties and methods from inside.

## Tables


## Functions, Methods and Objects

### Creating an object: constructor notation:
``` js
vor place = new Object();

place.name = 'A Place';
place.rooms = 10;
place.isPublic = true;

place.checkSomething = function() { // A method
  return this.isPublic;
  }
```
### Updating object
- To update value of proerties, use dot notation or square brackets.
- To delete a property, use delete keyword.

### Creating many objects, Constructor notation

- At times you will want several objects to represent similar things
- Object constructors can use a function as a template for creating objects.
- The uppercase in the function keyword is used as a reminder to use the new keyword when they create an object using that function.
``` js
function Hotel(name, rooms, booked) {
  this.name = name;
  this.rooms = rooms;
  this.booked = booked;
  
  this.checkAvailability = function() {
    return this.rooms - this.booked;
    }
  }
```

### Adding and removing properties
- Add and remove properties with dot notation.
``` js
var hotel = {
  name: 'place',
  rooms: 135,
  booked: 65
};

hotel.gym = true;
hotel.pool = false;
delete hotel.rooms;
```

### "This" keyword
- Commonly used inside function and objects. 
- Where the function is declared alters what "this" means. It always refers to one object, usually the object in which the function operates.

### Storing Data
- Variables have just one key (variable name)
- Arrays can store multiple pieces of info. Each piece separated by comma.
- Individual objects store sets of names/value pairs, either properties or methods.
- Multiple objects - when needing to create multiple objects within same page, you should use object constructor to privde template.

### Built-in Objects
- Browsers come with a set of built-in objects that represent browser window, current webpage shown, e.t.c.
- They allow you to get a wide amount of information from the browser based on the object type.
- Document.getElementById is an example.
- Three groups of built-in objects:
  - Browser Object Model (window, history, location, navigator, screen)
  - Document Object Model (document, html, head, body)
  - Global Javascript Objects (String, Number, Boolean)
- Math is an object as well, to create random numbers.

## Tables
- When representing table info, think in terms of a grid made up of rows and columns (such as a spreadsheet)

### What is a table?
- represents info in a grid format, examples of tables include financial reports, sports results.

### Basic Table Structure
- Table row is tr
- Table heading is th
- Table data is td, represents the actual data
``` html5
<table>
  <th scope="col">Monday</th>
  <th scope="col">Tuesday</th>
  <tr>
    <th scope="row">Things</th>
    <td>15</td>
    <td>15</td>
    <td>30</td>
    <td>17</td>
  </tr>
  <tr>
    <th scope="row">Things</th>
    <td>61</td>
    <td>2136</td>
    <td>32135</td>
    <td>324</td>
  </tr>
  <tr>
    <th scope="row">Things</th>
    <td>12346</td>
    <td>9643</td>
    <td>9632</td>
    <td>8126</td>
  </tr>
    <th scope="row">Things</th>
    <td>89126</td>
    <td>996</td>
    <td>699</td>
    <td>12</td>
  </tr>
</table>
```

### Spanning Columns
- using rowspan="numbervalue" and colspan="numbervalue" can scope them to different sizes.

### Long Tables
- Headings inside of the element should sit inside the thead element.
- Body should sit inside tbody
- tfoot is the foot of the element.
