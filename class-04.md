Read: 04 - HTML Links, CSS Layout, JS Functions



Links are the defining feature of the web
because they allow you to move from
one web page to another — enabling the
very idea of browsing or surfing.





Links are created using the <a> element. Users can click on anything
between the opening <a> tag and the closing </a> tag. You specify
which page you want to link to using the href attribute.


	<a> 

Links are created using the a
element which has an attribute
called href. The value of the
href attribute is the page that
you want people to go to when
they click on the link.


On larger websites it's a good idea to organize your code by placing the
pages for each different section of the site into a new folder. Folders on a
website are sometimes referred to as directories.


Relative URLs can be used when linking to pages within your own
website. They provide a shorthand way of telling the browser where to
find your files.


Relative Link Type
* Same Folder
* Child Folder
* Grandchild Folder
* Parent Folder
* GrandParent Folder






	mailto: 
To create a link that starts up
the user's email program and
addresses an email to a specified
email address, you use the a
element. However, this time the
value of the href attribute starts
with mailto: and is followed by
the email address you want the
email to be sent to.



	target
If you want a link to open in a
new window, you can use the
target attribute on the opening
a tag. The value of this
attribute should be _blank.




Links are created using the a element.
* The <a> element uses the href attribute to indicate
the page you are linking to.
* If you are linking to a page within your own site, it is
best to use relative links rather than qualified URLs.
* You can create links to open email programs with an
email address in the "to" field.
* You can use the id attribute to target elements within
a page that can be linked to



### Building Blocks
CSS treats each HTML element as if it is in its
own box. This box will either be a block-level
box or an inline box.



### Containing Elements
If one block-level element sits inside another
block-level element then the outer box is
known as the containing or parent element.



CSS has the following positioning schemes that allow you to control
the layout of a page: normal flow, relative positioning, and absolute
positioning. You specify the positioning scheme using the position
property in CSS. You can also float elements using the float property.


To indicate where a box should be positioned, you may also need to use
box offset properties to tell the browser how far from the top or bottom
and left or right it should be placed. (You will meet these when we
introduce the positioning schemes on the following pages.)


Normal Flow
* position:static

Relative Positioning
* position:relative


Absolute Positioning
* position:absolute


Fixed Positioning
* position:fixed


Overlapping Elements
* z-index


Floating Elements
* float


Clearing Floats
* clear

Many web pages use multiple
columns in their design. This
is achieved by using a <div>
element to represent each
column. The following three CSS
properties are used to position
the columns next to each other

* width
* float
* margin




Different visitors to your site will have different sized screens that show
different amounts of information, so your design needs to be able to
work on a range of different sized screens.



Resolution refers to the number of dots a screen shows per inch. Some
devices have a higher resolution than desktop computers and most
operating systems allow users to adjust the resolution of their screens


Because screen sizes and display resolutions vary so much, web
designers often try to create pages of around 960-1000 pixels wide
(since most users will be able to see designs this wide on their screens)




Fixed width layout
designs do not
change size as the
user increases
or decreases
the size of their
browser window.
Measurements tend
to be given in pixels.



Liquid layout designs
stretch and contract
as the user increases
or decreases the
size of their browser
window. They tend to
use percentages.



The liquid layout uses
percentages to specify the width
of each box so that the design
will stretch to fit the size of the
screen.




Composition in any visual art (such as design, painting, or photography)
is the placement or arrangement of visual elements — how they are
organized on a page. Many designers use a grid structure to help them
position items on a page, and the same is true for web designers.




CSS frameworks aim to make your life easier by providing the code for
common tasks, such as creating layout grids, styling forms, creating
printer-friendly versions of pages and so on. You can include the CSS
framework code in your projects rather than writing the CSS from scratch.


Below you can see a sample layout of a page just like the fixed width
page example. On the next page, we will recreate this using the 960.gs
stylesheet. Instead of writing our own CSS to control layout, we will need
to add classes to the HTML indicating how wide each section should be.


There are two ways to add
multiple style sheets to a page:


1: Your HTML page can link
to one style sheet and that
stylesheet can use the @import
rule to import other style sheets.

2: In the HTML you can use a
separate link element for
each style sheet.



On this page you can see the
other technique for including
multiple style sheets. Inside the
head element is a separate
link element for each style
sheet.




div elements are often used as containing elements
to group together sections of a page.
* Browsers display pages in normal flow unless you
specify relative, absolute, or fixed positioning.
* The float property moves content to the left or right
of the page and can be used to create multi-column
layouts. (Floated items require a defined width.)
* Pages can be fixed width or liquid (stretchy) layouts.
* Designers keep pages within 960-1000 pixels wide,
and indicate what the site is about within the top 600
pixels (to demonstrate its relevance without scrolling).
* Grids help create professional and flexible designs.
* CSS Frameworks provide rules for common tasks.
* You can include multiple CSS files in one page.





Browsers require very detailed instructions about what
we want them to do. Therefore, complex scripts can run
to hundreds (even thousands) of lines. Programmers use
functions, methods, and objects to organize their code.
This chapter is divided into three sections that introduce: 




* FUNCTIONS METHODS 
* OBJECTS
* BUILT-IN OBJECTS 



Functions let you group a series of statements together to perform a
specific task. If different parts of a script repeat the same task, you can
reuse the function (rather than repeating the same set of statements). 



Functions can return more than one value using an array.
For example, this function calculates the area and volume of a box. 



Expressions produce a value. They can be used where values are expected.
If a function is placed where a browser expects to see an expression,
(e.g., as an argument to a function), then it gets treated as an expression



This way of writing a function is used in several different situations.
Often functions are used to ensure that the variable names do not conflict
with each other (especially if the page uses more than one script). 



	var area = (ltuncti on()
	var wi dth = 3;
	var height = 2;
	return widt h * height;
	}DI);


The location where you declare a variable will affect where it can be used
within your code. If you declare it within a function, it can only be used
within that function. This is known as the variable's scope.


Global variables use more memory. The browser has to remember them
for as long as the web page using them is loaded. Local variables are only
remembered during the period of time that a function is being executed.



### Why pair program?


1. Greater efficiency
2. Engaged collaboration
3. Learning from fellow students
4. Social skills
5. Job interview readiness
6. Work environment readiness



### BOOKS USED:

1. HTML AND CSS: https://wtf.tw/ref/duckett.pdf

2. javascript and jquery interactive jon du

3. https://www.codefellows.org/blog/6-reasons-for-pair-programming/


