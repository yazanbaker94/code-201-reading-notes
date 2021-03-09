##  “Forms” 



Traditionally, the term 'form' has referred
to a printed document that contains
spaces for you to fill in information.



The best known form on the web is probably
the search box that sits right in the middle of
Google's homepag



There are several types of form controls that
you can use to collect information from visitors
to your site



A user fills in a form and then presses a button
to submit the information to the server.



A form may have several form controls, each
gathering different information. The server
needs to know which piece of inputted data
corresponds with which form element.


	form

Form controls live inside a
form element. This element
should always carry the action
attribute and will usually have a
method and id attribute too.
action


	action

Every form element requires
an action attribute. Its value
is the URL for the page on the
server that will receive the
information in the form when it
is submitted.
method



	method

Forms can be sent using one of
two methods: get or post.




	input

The input element is used
to create several different form
controls. The value of the type
attribute determines what kind
of input they will be creating.




	type="password"


When the type attribute has
a value of password it creates
a text box that acts just like a
single-line text input, except
the characters are blocked out.
They are hidden in this way so
that if someone is looking over
the user's shoulder, they cannot
see sensitive data such as
passwords.



	textarea


The textarea element
is used to create a mutli-line
text input. Unlike other input
elements this is not an empty
element. It should therefore have
an opening and a closing tag.



	input

type="radio"
Radio buttons allow users to pick
just one of a number of options.



	input

type="checkbox"
Checkboxes allow users to select
(and unselect) one or more
options in answer to a question.




	select


A drop down list box (also
known as a select box) allows
users to select one option from a
drop down list. 



	select

	size


You can turn a drop down select
box into a box that shows more
than one option by adding the
size attribute. Its value should
be the number of options you
want to show at once. In the
example you can see that three
of the four options are shown.



	input

If you want to allow users to
upload a file (for example an
image, video, mp3, or a PDF),
you will need to use a file input
box.


	type="submit"


The submit button is used to
send a form to the server.



	input


type="image"
If you want to use an image for
the submit button, you can give
the type attribute a value of
image. The src, width, height,
and alt attributes work just
like they do when used with the
img element 


	button


The button element was
introduced to allow users more
control over how their buttons
appear, and to allow other
elements to appear inside the
button



	label


When introducing form controls,
the code was kept simple by
indicating the purpose of each
one in text next to it. However,
each form control should have
its own label element as this
makes the form accessible to
vision-impaired users.




	fieldset
You can group related form
controls together inside the
fieldset element. This is
particularly helpful for longer
forms.




	input
Many forms need to gather
information such as dates, email
addresses, and URLs. This has
traditionally been done using
text inputs.




	input


HTML5 has also introduced
inputs that allow visitors to
enter email addresses and URLs.
Browsers that do not support
these input types will just treat
them as text boxes.




	input


If you want to create a single
line text box for search queries,
HTML5 provides a special type
of input for that purpose.






Whenever you want to collect information from
visitors you will need a form, which lives inside a
form element.


* Information from a form is sent in name/value pairs.
* Each form control is given a name, and the text the
user types in or the values of the options they select
are sent to the server.
* HTML5 introduces new form elements which make it
easier for visitors to fill in forms.


<hr>
<hr>
<hr>



The list-style-type property
allows you to control the shape
or style of a bullet point (also
known as a marker). 




You can specify an image to act
as a bullet point using the
list-style-image property



	list-style-position



Lists are indented into the page
by default and the list-styleposition property indicates
whether the marker should
appear on the inside or the
outside of the box containing the
main points. 


	list-style


As with several of the other CSS
properties, there is a property
that acts as a shorthand for list
styles. It is called list-style,
and it allows you to express
the markers' style, image and
position properties in any order.




## Table Properties


width to set the width of the
table

padding to set the space
between the border of each table
cell and its content

text-transform to convert the
content of the table headers to
uppercase

letter-spacing, font-size
to add additional styling to the
content of the table headers

border-top, border-bottom
to set borders above and below
the table headers

text-align to align the writing
to the left of some table cells and
to the right of the others


background-color to change
the background color of the


alternating table rows


:hover to highlight a table row
when a user's mouse goes over it





	empty-cells

If you have empty cells in
your table, then you can use
the empty-cells property to
specify whether or not their
borders should be shown.



	border-spacing, border-collapse


The border-spacing property
allows you to control the
distance between adjacent cells.
By default, browsers often leave
a small gap between each table
cell, so if you want to increase
or decrease this space then
the border-spacing property
allows you to control the gap.


	cursor


The cursor property allows
you to control the type of mouse
cursor that should be displayed
to users.




In addition to the CSS properties covered in other
chapters which work with the contents of all elements,
there are several others that are specifically used to
control the appearance of lists, tables, and forms.


* List markers can be given different appearances
using the list-style-type and list-style image
properties.

* Table cells can have different borders and spacing in
different browsers, but there are properties you can
use to control them and make them more consistent.

* Forms are easier to use if the form controls are
vertically aligned using CSS.

* Forms benefit from styles that make them feel more
interactive.



<hr>
<hr>
<hr>



When you browse the web, your browser registers different
types of events. It's the browser's way of saying, "Hey, this
just happened." Your script can then respond to these events



Here is a selection of the events that occur in the browser while you are
browsing the web. Any of these events can be used to trigger a function
in your JavaScript code. 



When the user interacts with the HTML on a web page, there are three
steps involved in getting it to trigger some JavaScript code.
Together these steps are known as event handling. 



1. Select t he element
node(s) you want the
script to respond to. 


2. Indicate which event on
the selected node(s) will
trigger the response. 



3. State the code you want
to run when the event
occurs. 




Event handlers let you indicate which event you
are waiting for on any particular element.
There are three types of event handlers. 




1. HTML EVENT
HANDLERS 

2. TRADITIONAL DOM
EVENT HANDLERS

3. DOM LEVEL 2 EVENT
LISTENERS 



All modern browsers understand this way of creating an event handler,
but you can only attach one function to each event handler. 


Event listeners are a more recent approach to handling events.
They can deal with more than one function at a time
but they are not supported in older browsers. 



Because you cannot have parentheses after the
function names in event handlers or listeners,
passing arguments requires a workaround. 



IES-8 had a different event model and did not support
addEventL i stener() but you can provide fallback code
to make event listeners work with older versions of IE. 


When an event occurs, the event object tells
you information about the event, and the
element it happened upon. 


Below you can see how you get the event object in IES-8.
It is not passed automatically to event handler/listener functions;
but it is available as a child of the window object. 




Creating event listeners for a lot of elements
can slow down a page, but event flow allows
you to listen for an event on a parent element. 





The event object has methods that change:
the default behavior of an element and how
the element's ancestors respond to the event. 




1. preventDefau1t () 
2. stopPropagation() 
3. USING BOTH METHODS 




When calling a function, the event object's target property is the best
way to determine which element the event occurred on. But you may see
the approach below used; it relies on the this keyword. 



User interface CUI) events occur as a result of interaction with the
browser window rather than the HTML page contained within it,
e.g., a page having loaded or the browser window being resized. 


![UI](https://i.ibb.co/ThvFPrb/validatorhtml.png
)

The HTML elements you can interact with, such as links and form
elements, can gain focus. These events fire when they gain or lose focus. 




The mouse events are fired when the mouse is moved and also when its
buttons are clicked.





The keyboard events are fired when a user interacts with the keyboard
(they fire on any kind of device with a keyboard). 






There are two events that are commonly used with forms.
In particular you are likely to see submit used in form validation. 







Whenever elements are added to or removed from the DOM, its
structure changes. This change triggers a mutation event. 






BOOKS/LINKS USED:

1. HTML AND CSS - DUCKETT 
2. javascript and jquery interactive jon du
