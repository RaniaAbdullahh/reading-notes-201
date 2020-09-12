# Understanding The Problem Domain Is The Hardest Part Of Programming
## What is the hardest thing about writing code?

- Learning a new technology.
- Naming things
- Testing your code
- Debugging
- Fixing bugs
- Making software maintainable
>Very simple functionality, easily explainable, but most importantly, easily understood.
What I found with this simple application was that because it was so easy to understand, the focus was taken off of the problem domain and put instead on the technology.
## Why problem domains are hard
Simply that by taking away the problem domain, or making it so trivial that it is easily understood, I am able to make both teaching and learning easier.
The real world is a messy place.  Many of the problem domains we face as programmers are difficult to understand and look completely different depending on your viewpoint.
As programmers, we also are often not given complete information about the problem domain, so we don’t even have the information we need to understand it.
## Programming is easy if you understand the problem domain
You can often make the problem domain easier by cutting out cases and narrowing your focus to a particular part of the problem.
It is easy to fall into the trap of thinking you understand enough of the problem to get started coding it.

# Object Literals
Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object,
variables and functions take on new names
- CREATING· OBJECTS USING LITERAL NOTATION 
This example starts by creating an object using literal notation.
This object is called hotel which represents a hotel called Quay with 40 rooms (25 of which have been booked).
Next, the content of the page is updated with data from this object. It shows the name of the hotel by accessing the object's name property and the number
of vacant rooms using the ```checkAvail ability()``` method.
To access a property of this object, the object name is followed by a dot (the period symbol) and the name of the property that you want.
Similarly, to use the method, you can use the object name followed by the method name.
```hotel.checkAvailability()```
If the method needs parameters, you can supply them in the parentheses (just like you can pass arguments to a function). 
```
var hote l = {
name: 'Quay',
rooms: 40,
booked : 25,
checkAvailability: function() {
return this.rooms - this.booked;
}
} ;
JAVASCRIPT
var el Name = document .getElementByld('hotelName');
elName.textContent =hotel .name;
var elRooms = document.getElementByid{'rooms');
elRooms.textContent = hotel .checkAvailability();  
```
# The Document Object Model (DOM) 
(DOM)  specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.
>The browser represents the page using a DOM tree.

>DOM trees have four types of nodes: document nodes, element nodes, attribute nodes, and text nodes.

>You can select element nodes by their id or cl ass attributes, by tag name, or using CSS selector syntax.

>Whenever a DOM query can return more than one node, it will always return a Nadel i st.

>From an element node, you can access and update its content using properties such as textContent and i nnerHTML or using DOM manipulation techniques.

>An element node can contain multiple text nodes and child elements that are siblings of each other.

>In older browsers, implementation of the DOM is inconsistent (and is a popular reason for using jQuery).

>Browsers offer tools for viewing the DOM tree . 
