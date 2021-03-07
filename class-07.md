### Define a constructor and initialize properties
To define the same properties between many objects, you'll want to use a constructor function. Below is a table that summarizes a JavaScript representation of an EpicFailVideo object.


var EpicFailVideo = function(epicRating, hasAnimals) {
  this.epicRating = epicRating;
  this.hasAnimals = hasAnimals;
}

    var EpicFailVideo = function(epicRating, hasAnimals) {
      this.epicRating = epicRating;
      this.hasAnimals = hasAnimals;
    }
    
    var parkourFail = new EpicFailVideo(7, false);
    var corgiFail = new EpicFailVideo(4, true);
    
    console.log(parkourFail);
    console.log(corgiFail);





This is object-oriented programming in JavaScript at its most fundamental level.

1. The new keyword instantiates (i.e. creates) an object.
2. The constructor function initializes properties inside that object using the this variable.
3. The object is stored in a variable for later use.



Here's some tips to follow when building your own domain models.



1. When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
2. Model its attributes with a constructor function that defines and initializes properties.
3. Model its behaviors with small methods that focus on doing one job well.
4. Create instances using the new keyword followed by a call to a constructor function.
5. Store the newly created object in a variable so you can access its properties and methods from outside.
6. Use the this variable within methods so you can access the object's properties and methods from inside.




hr
hr

A table represents information in a grid format.
Examples of tables include financial reports, TV
schedules, and sports results.



	table


The table element is used
to create a table. The contents
of the table are written out row
by row.

	tr


You indicate the start of each
row using the opening tr tag.
(The tr stands for table row.)
It is followed by one or more
td elements (one for each cell
in that row).
At the end of the row you use a
closing /tr tag.


	td


Each cell of a table is
represented using a td
element. (The td stands for
table data.)
At the end of each cell you use a
closing /td tag.



	th


The th element is used just
like the td element but its
purpose is to represent the
heading for either a column or
a row. (The th stands for table
heading.) 



	thead


The headings of the table should
sit inside the thead element.

	tbody


The body should sit inside the
tbody element.


	tfoot
The footer belongs inside the
tfoot element.




The table element is used to add tables to a web
page.
* A table is drawn out row by row. Each row is created
with the tr element.
* Inside each row there are a number of cells
represented by the td element (or th if it is a
header).
* You can make cells of a table span more than one row
or column using the rowspan and colspan attributes.
* For long tables you can split the table into a thead,
tbody, and tfoot




hr
<hr>



Sometimes you will want several objects to represent similar things.
Object constructors can use a function as a template for creating objects.
First, create the template with the object's properties and methods


The keyword this is commonly used inside functions and objects.
Where the function is declared alters what this means. It always refers
to one object, usually the object in which the function operates. 




In JavaScript, data is represented using name/value pairs.
To organize your data, you can use an array or object to group a set of
related values. In arrays and objects the name is also known as a key. 




If you want to access items via a property name or key, use an object
(but note that each key in the object must be unique).
If the order of the items is important, use an array. 




The window object represents the current
browser window or tab. It is the topmost object
in the Browser Object Model, and it contains
other objects that tell you about the browser. 


The topmost object in the Document Object Model (or DOM) is the
document object. It represents the web page loaded into the current
browser window or tab. You meet its child objects in Chapter 5. 

Whenever you have a value that is a string, you can use the properties
and methods of the String object on that value. This example stores the
phrase "Home sweet home " in a variable


Each character in a string is automatically given a number, called an index
number. Index numbers always start at zero and not one (just like for
items in an array). 



In JavaScript there are six data types:
Five of them are described as simple (or primitive) data types.
The sixth is the object (and is referred to as a complex data type). 


Whenever you have a value that is a number,
you can use the methods and properties of the
Number object on it. 


The Math object has properties and methods
for mathematical constants and functions


* Functions allow you to group a set of related
statements together that represent a single task.

* Functions can take parameters (informatiorJ required
to do their job) and may return a value.

* An object is a series of variables and functions that
represent something from the world around you.

* In an object, variables are known as properties of the
object; functions are known as methods of the object.

* Web browsers implement objects that represent both
the browser window and the document loaded into the
browser window.

* JavaScript also has several built-in objects such as
String, Number, Math, and Date. Their properties and
methods offer functionality that help you write scripts.

* Arrays and objects can be used to create complex data
sets (and both can contain the other). 






BOOKS/LINKS USED:


https://github.com/codefellows/domain_modeling#domain-modeling

