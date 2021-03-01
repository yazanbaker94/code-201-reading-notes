
# Chapter 3: “Lists”




* Ordered lists are lists where each item in the list is
numbered. For example, the list might be a set of steps for
a recipe that must be performed in order, or a legal contract
where each point needs to be identified by a section
number.
* Unordered lists are lists that begin with a bullet point
(rather than characters that indicate order).
* Definition lists are made up of a set of terms along with the
definitions for each of those terms.


	<ol>
The ordered list is created with
the ol element.
	<li>
Each item in the list is placed
between an opening li tag
and a closing /li tag. (The li
stands for list item.)


	<ul>
The unordered list is created
with the ul element.
	<li>
Each item in the list is placed
between an opening li tag
and a closing /li tag. (The li
stands for list item.)


	<dl>
The definition list is created with
the dl element and usually
consists of a series of terms and
their definitions.

Inside the dl element you will
usually see pairs of dt and
dd elements.

	<dt>
This is used to contain the term
being defined (the definition
term).
	<dd>
This is used to contain the
definition.
Sometimes you might see a list
where there are two terms used
for the same definition or two
different definitions for the same
term.




###	There are three types of HTML lists: ordered,
unordered, and definition.
* Ordered lists use numbers.
* Unordered lists use bullets.
* Definition lists are used to define terminology.
* Lists can be nested inside one another





<hr>
<hr>
<hr>


By default a box is sized just big
enough to hold its contents. To
set your own dimensions for a
box you can use the height and
width properties.


By default a box is sized just big
enough to hold its contents. To
set your own dimensions for a
box you can use the height and
width properties.


Some page designs expand and
shrink to fit the size of the user's
screen. In such designs, the
min-width property specifies
the smallest size a box can be
displayed at when the browser
window is narrow, and the
max-width property indicates
the maximum width a box can
stretch to when the browser
window is wide.


In the same way that you might
want to limit the width of a box
on a page, you may also want
to limit the height of it. This is
achieved using the min-height
and max-height properties.



The overflow property tells the
browser what to do if the content
contained within a box is larger
than the box itself. It can have
one of two values:

1. hidden

This property simply hides any
extra content that does not fit in
the box.

2. scroll

This property adds a scrollbar to
the box so that users can scroll
to see the missing content.

Every box has three available properties that
can be adjusted to control its appearance:

1. Border
2. Margin
3. Padding




The border-width property
is used to control the width
of a border. The value of this
property can either be given
in pixels or using one of the
following values:

1. thin
2. medium
3. thick



You can control the style of a
border using the border-style
property. This property can take
the following values:


1. solid
2. dotted
3. dashed
4. double
5. groove
6. ridge
7. inset
8. outset
9. hidden / none



You can specify the color of a
border using either RGB values,
hex codes or CSS color names



The border property allows you
to specify the width, style and
color of a border in one property
(and the values should be coded
in that specific order).



The padding property allows
you to specify how much space
should appear between the
content of an element and its
border. 


The margin property controls
the gap between boxes. Its value
is commonly given in pixels,
although you may also use
percentages or ems.



If you want to center a box on
the page (or center it inside
the element that it sits in), you
can set the left-margin and
right-margin to auto




The display property allows
you to turn an inline element
into a block-level element or vice
versa, and can also be used to
hide an element from the page.


1. inline
2. block
3. inline-block
4. none



The visibility property allows
you to hide boxes from users
but It leaves a space where the
element would have been.

1. hidden
2. visible




The border-image property
applies an image to the border of
any box. It takes a background
image and slices it into nine
pieces.



The box-shadow property
allows you to add a drop shadow
around a box. It works just like
the text-shadow property that
you met on page 288. It must
use at least the first of these two
values as well as a color:



1. Horizontal offset
2. Vertical offset
3. Blur distance
4. Spread of shadow


CSS3 introduces the ability to
create rounded corners on any
box, using a property called
border-radius. The value
indicates the size of the radius
in pixels.




CSS treats each HTML element as if it has its own box.
* You can use CSS to control the dimensions of a box.
* You can also control the borders, margin and padding
for each box with CSS.
* It is possible to hide elements using the display and
visibility properties.
* Block-level boxes can be made into inline boxes, and
inline boxes made into block-level boxes.
* Legibility can be improved by controlling the width of
boxes containing text and the leading.
* CSS3 has introduced the ability to create image
borders and rounded borders.





<hr>
<hr>
<hr>



An array is a special type of variable. It doesn't
just store one value; it stores a list of values. 



You should consider using an
array whenever you are working
with a list or a set of values that
are related to each other. 



You create an array and give it
a name just like you would any
other variable (using the var
keyword followed by the name of
the array). 



	var colors;
	colors ['white', 'black', ' custom'];
	var el document.getElementByld('col ors');
	el . textContent = col ors[O];



Values in an array are accessed as if they are in
a numbered list. It is important to know that the
numbering of this list starts at zero (not one). 



	var colors = ['white',
	'black' ,
	'custom'];
	// Update the third item in the array
	colors[2] = 'beige ' ;
	// Get the element with an id of col ors
	var el = document .getElementByid(' colors') ;
	// Replace with third item from the array
	el .textContent = colors[2];




<hr>

<hr>

<hr>




Here you can see that an
if ... e 1 se statement allows you
to provide two sets of code:
1. one set if the condition
evaluates to true
2. another set if the condition is
false 


	var pass = 50;
	var score = 75;
	var msg;
	if (score >= pass) {
	msg = 'Congratulations, you passed!';
	} else {
	msg = 'Have another go!';
	var el = document .getElementByld('answer');
	el .textContent = msg;




An if ... e 1 se statement runs one set of code if the
condition is true or a different set if it is fa 1 se: 




A switch statement starts with a
variable called the switch value.
Each case indicates a possible
value for this variable and the
code that should run if the
variable matches that value


If you use a data type JavaScript did not expect,
it tries to make sense of the operation rather
than report an error. 



Due to type coercion, every value in JavaScript
can be treated as if it were true or false; and
this has some interesting side effects.




Because the presence of an object or array can
be considered truthy, it is often used to check
for the existence of an element within a page. 




Logical operators are processed left to right.
They short-circuit (stop) as soon as they have a
result - but they return the value that stopped
the processing (not necessarily true or fa 1 se). 



### LOOPS KEYWORD:


1. break

2. continue



A for loop is often used to loop
through the items in an array.



The key difference between
a whi 1 e loop and a do whi 1 e
loop is that the statements in
the code block come before the
condition. This means that those
statements are run once whether
or not the condition is met. 





Conditional statements allow your code to make
decisions about what to do next.

Comparison operators (===, ! ==, ==, ! =, <, >, <=, =>)
are used to compare two operands.

Logical operators allow you to combine more than one
set of comparison operators.

if ... else statements allow you to run one set of code
if a condition is true, and another if it is false.

switch statements allow you to compare a value
against possible outcomes (and also provides a default
option if none match).

Data types can be coerced from one type to another.
All values evaluate to either truthy or falsy.
There are three types of loop: for, while, and
do ... while. Each repeats a set of statements. 
