# Domain Modeling

A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams.

**Define a constructor and initialize properties**

To define the same properties between many objects, you'll want to use a constructor function

This is object-oriented programming in JavaScript at its most fundamental level.

The new keyword instantiates (i.e. creates) an object.
The constructor function initializes properties inside that object using the this variable.
The object is stored in a variable for later use.

* When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.

* Model its attributes with a constructor function that defines and initializes properties.

* Model its behaviors with small methods that focus on doing one job well.

* Create instances using the new keyword followed by a call to a constructor function.

* Store the newly created object in a variable so you can access its properties and methods from outside.

* Use the this variable within methods so you can access the object's properties and methods from inside.

# Tables

* The table element is used to add tables to a web
page.

* A table is drawn out row by row. Each row is created
with the tr element.

* Inside each row there are a number of cells
represented by the td element (or th if it is a
header).

* You can make cells of a table span more than one row
or column using the rowspan and colspan attributes.

* For long tables you can split the table into a (thead,
tbody, and tfoot)

# Functions, Methods, and Objects

**WAYS TOCREATE OBJECTS**

1- CREATE THE OBJECT, THEN ADD PROPERTIES & METHODS

> var hotel = {}

2- CREATING AN OBJECT WITH PROPERTIES & METHODS

> var hotel = {
name: 'Quay' ,
rooms: 40,
booked: 25,
chec kAvailability: function() {
return this.rooms - this .booked;
}
} ;

**THIS (IT IS A KEYWORD)**

The keyword this is commonly used inside functions and objects.
Where the function is declared alters what this means. It always refers
to one object, usually the object in which the function operates.

1- A FUNCTION IN GLOBAL SCOPE

When a function is created at the top level of a script
(that is, not inside another object or function), then it
is in the global scope or global context.

2- GLOBAL VARIABLES

All global variables also become properties of the
window object. so when a function is in the global
context, you can access global variables using the
window object, as well as its other properties.


**BUILT-IN OBJECTS**

Browsers come with a set of built-in objects that represent things like the
browser window and the current web page shown in that window. These
built-in objects act like a toolkit for creating interactive web pages.

