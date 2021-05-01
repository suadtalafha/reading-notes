# Summary 
## WHAT IS AN OBJECT?

Objects: group together a set of variables and functions to create a model
of a something you would recognize from the real world. In an object,
variables and functions take on new names.

In JavaScript:
* Variables have a name and you can assign them a
value of a string, number, or Boolean.
* Arrays have a name and a group of values. (Each
item in an array is a name/value pair because it
has an index number and a value.)
* Named functions have a name and value that is a
set of statements to run if the function is called.
* Objects consist of a set of name/value pairs
(but the names are referred to as keys).

Example 
var hotel = {
name: 'Quay',
rooms : 40,
booked: 25,
checkAvailability: function() {
return this.rooms - this.booked;
}
} ;
JAVASCRIPT
var elName = document .getElementByld('hotelName');
elName.textContent =hotel .name;
var elRooms = document.getElementByid{'rooms');
elRooms .textContent = hotel .checkAvailability();


![image](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRV-Js-4lWZE70rAs0tP6bXYhA4uuXZCRuFNQ&usqp=CAU.jpg)


# Summay
## Document object model 
* The browser represents the page using a DOM tree.
DOM trees have four types of nodes: document nodes,
element nodes, attribute nodes, and text nodes.
* You can select element nodes by their id or cl ass
attributes, by tag name, or using CSS selector syntax.
* Whenever a DOM query can return more than one
node, it will always return a Nadel i st.
* From an element node, you can access and update its
content using properties such as textContent and
i nnerHTML or using DOM manipulation techniques.
* An element node can contain multiple text nodes and
child elements that are siblings of each other.
* In older browsers, implementation of the DOM is
inconsistent (and is a popular reason for using jQuery).
Browsers offer tools for viewing the DOM tree .

![image](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQM7LOofqTdy2EBnd3OlGA0INuGcvmgADDSxQ&usqp=CAU.jpg)