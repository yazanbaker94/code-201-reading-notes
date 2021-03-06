"What I found with this simple application was that because it was so easy to understand, the focus was taken off of the problem domain and put instead on the technology."


"By creating a familiar problem domain, I found that both the tasks of me teaching a new technology and the viewer learning that technology were much easier, because it is very difficult to learn more than one thing at once."

"The real world is a messy place.  Many of the problem domains we face as programmers are difficult to understand and look completely different depending on your viewpoint."


### Programming is easy if you understand the problem domain


"I was easily able to learn that problem domain and because of it, I was able to write the code very easily as well"


### What can you do about it?


If understanding the problem domain is the hardest part of programming and you want to make programming easier, you can do one of two things:

Make the problem domain easier
Get better at understanding the problem domain


"You can often make the problem domain easier by cutting out cases and narrowing your focus to a particular part of the problem."


"So many developers don’t realize how much of an impact marketing themselves and branding can have on their opportunities.  I’m hoping to help developers learn not only how valuable marketing and branding is, but how to do it most effectively."



<hr>
<hr>
<hr>


Objects group together a set of variables and functions to create a model
of a something you would recognize from the real world. In an object,
variables and functions take on new names. 



This object represents a hotel. It has five properties and one method.
The object is in curly braces. It is stored in a variable called hotel . 

<hr>
<hr>



The Document Object Model (DOM) specifies
how browsers should create a model of an HTML
page and how JavaScript can access and update the
contents of a web page while it is in the browser window.




As a browser loads a web page, it creates a model of that page.
The model is called a DOM tree, and it is stored in the browsers' memory.
It consists of four main types of nodes. 




Each node is an object with methods and properties.
Scripts access and update this DOM tree (not the source HTML file).
Any changes made to the DOM tree are reflected in the browser. 



Accessing and updating the DOM tree involves two steps:
1: Locate the node that represents the element you want to work with.
2: Use its text content, child elements, and attributes. 





	get ElementByld ()


Uses the value of an element's
id attribute (which should be
unique within the page).
See p195 



	querySe1ector ()


Uses a CSS selector, and returns
the first matching element.
See p202 


	getElementsByClassName()


Selects all elements that have
a specific value for their cl ass
attribute. 



	getElementsByTagName()


Selects all elements that have the
specified tag name ..




	querySelectorAll()


Uses a CSS selector to select all
matching elements.



	firstChild / lastChild


Select the first or last child of the
current element. 




The terms elements and element nodes are used interchangeably
but when people say the DOM is working with an element,
it is actually working with a node that represents that element. 



DOM queries may return one element, or they may return a Nodelist,
which is a collection of nodes. 



When a DOM method can return more than one element, it returns a
Nodelist (even if it only finds one matching element). 




Here you can see four different DOM queries that all return a Nodelist.
For each query, you can see the elements and their index numbers in the
Nodelist that is returned. 



There are two ways to select an element from a Nodelist:
The item() method and array syntax.
Both require the index number of the element you want. 



When you have an element node, you can select
another element in relation to it using these five
properties. This is known as traversing the DOM. 


Traversing the DOM can be difficult because
some browsers add a text node whenever they
come across whitespace between elements. 


When you select a text node, you can retrieve or amend the content of it
using the node Va 1 ue property




The textContent property allows you to
collect or update just the text that is in the
containing element (and its children). 


Using the i nnerHTML property, you can access
and amend the contents of an element,
including any child elements.


DOM manipulation offers another technique
to add new content to a page (rather than
i nnerHTML). It involves three steps: 


1. CREATE THE ELEMENT - createEl ement ()


2. GIVE IT CONTENT  - createTextNode() 

3. ADD IT TO THE DOM - appendChild() 


DOM manipulation can be used to remove
elements from the DOM tree


STORE THE ELEMENT
TO BE REMOVED IN A
VARIABLE 


STORE THE PARENT OF
THAT ELEMENT IN A
VARIABLE 



REMOVE THE ELEMENT
FROM ITS CONTA INING
ELEMENT



So far, you have seen three techniques for adding HTML to a web page.
It's time to compare when you should use each one. 



You can choose different techniques depending on the task (and keep in
mind how the site might be developed in the future). 


you need to be aware of Cross-Site Scripting Attacks or XSS; otherwise,
an attacker could gain access to your users' accounts. 


VALIDATE INPUT GOING TO THE SERVER 


1. Only let visitors input the kind
of characters they need to when
supplying information. This is
known as validation. Do not
allow untrusted users to submit
HTML markup or JavaScript.



2. Double-check validation on
the server before displaying user
content/storing it in a database.
This is important because users
could bypass validation in the
browser by turning JavaScript off. 


3. The database may safely
contain markup and script
from trusted sources (e.g., your
content management system).
This is because it does not try to
process the code; it just stores it. 



ESCAPE DATA COMING FROM THE SERVER & DATABASE 



6. Do not create DOM fragments
containing HTML from untrusted
sources. It should only be added
as text once it has been escaped


5. Make sure that you are only
inserting content generated by
users into certain parts of the
template files  


4. As your data leaves the
database, all potentially
dangerous characters should be
escaped 




Make sure that your users can only input characters they need to use
and limit where this content will be shown on the page. 



Any content generated by users that contain characters that are used
in code should be escaped on the server. You must control any markup
added to the page. 


Modern browsers come with tools that help
you inspect the page loaded in the browser
and understand the structure of the DOM tree


* The browser represents the page using a DOM tree.
* DOM trees have four types of nodes: document nodes,
element nodes, attribute nodes, and text nodes.
* You can select element nodes by their id or cl ass
attributes, by tag name, or using CSS selector syntax.
* Whenever a DOM query can return more than one
node, it will always return a Nadel i st.
* From an element node, you can access and update its
content using properties such as textContent and
innerHTML or using DOM manipulation techniques.
* An element node can contain multiple text nodes and
child elements that are siblings of each other.
* In older browsers, implementation of the DOM is
inconsistent (and is a popular reason for using jQuery).
* Browsers offer tools for viewing the DOM tree . 

BOOKS USED:

1. javascript and jquery interactive jon du
2. http://simpleprogrammer.com/2013/07/15/understanding-the-problem-domain-is-the-hardest-part-of-programming



