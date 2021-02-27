# Read: 01 - Introductory HTML and JavaScript


All websites use HTML and CSS, but content management systems, blogging software, and e-commerce platforms often add a few more technologies into the mix

When you visit a website, the web server hosting that site could be anywhere in the world. In order for you to find the location of the web server, your browser will first connect to a Domain Name System (DNS) server.

Tags act like containers. They tell you something about the information that lies between their opening and closing tags.

Attributes provide additional information about the contents of an element. They appear on the opening tag of the element and are made up of two parts: a name and a value, separated by an equals sign.

HTML5 allows you to use uppercase attribute names and omit the quotemarks, but this is not recommended.

HTML pages are text documents.
* HTML uses tags (characters that sit inside angled
brackets) to give the information they surround special
meaning.
* Tags are often referred to as elements.
* Tags usually come in pairs. The opening tag denotes
the start of a piece of content; the closing tag denotes
the end.
* Opening tags can carry attributes, which tell us more
about the content of that element.
* Attributes require a name and a value.
* To learn HTML you need to know what tags are
available for you to use, what they do, and where they
can go.



Since the web was first created, there have been several different versions of HTML.

HTML 4
Released 1997


XHTML 1.0
Released 2000


HTML5
Released 2000



If you want to add a comment to your code that will not be visible in the user's browser, you can add the text between these characters: 
        <!-- comment goes here -->


Every HTML element can also carry a class attribute. Sometimes, rather than uniquely identifying one element within a document, you will want a way to identify several elements as being different from the other elements on the page. For example, you might have some paragraphs of text that contain information that is more important than others and want to distinguish these elements, or you might want to differentiate between links that point to other pages on your own site and links that point to external sites.



Some elements will always appear to start on a new line in the browser window. These are known as block level elements. 


Some elements will always appear to continue on the same line as their neighbouring elements. These are known as inline elements.


        <div>
 This element allows you to
group a set of elements together
in one block-level box.
For example, you might create
a <div> element to contain all
of the elements for the header
of your site (the logo and the
navigation), or you might create
a <div> element to contain
comments from visitors.
  
  
        <span>
The span element acts like
an inline equivalent of the <div>
element. It is used to either:
1. Contain a section of text
where there is no other suitable
element to differentiate it from
its surrounding text
2. Contain a number of inline
elements
The most common reason why
people use <span> elements
is so that they can control the
appearance of the content of
these elements using CSS.
  
  
        <iframe>
An iframe is like a little window
that has been cut into your
page — and in that window you
can see another page. The term
iframe is an abbreviation of inline
frame.

        src
The src attribute specifies the
URL of the page to show in the
frame.

        height
The height attribute specifies
the height of the iframe in pixels.

        width
The width attribute specifies
the width of the iframe in pixels.


        seamless
In HTML5, a new attribute
called seamless can be applied
to an iframe where scrollbars
are not desired. The seamless
attribute (like some other new
HTML5 attributes) does not
need a value, but you will often
see authors give it a value of
seamless. Older browsers
do not support the seamless
attribute


         <meta>
The <meta> element lives
inside the <head> element and
contains information about that
web page.
  
  
description
keywords
robots
author
pragma
expires


There are some characters that are used in and reserved by HTML code. (For example, the left and right angled brackets.)


### DOCTYPES tell browsers which version of HTML you are using.
* You can add comments to your code between the
 comments markers.
* The id and class attributes allow you to identify
particular elements.
* The div and <span> elements allow you to group
block-level and inline elements together.
* iframes cut windows into your web pages through
which other pages can be displayed.
* The meta tag allows you to supply all kinds of
information about your web page.
* Escape characters are used to include special
characters in your pages such as <, >, and ©.
  
  
For a long time, web page authors used div elements to group together related elements on the page (such as the elements that form a header, an article, footer or sidebar). Authors used class or id attributes to indicate the role of the div element in the structure of the page.
 
 
HTML5 introduces a new set of elements that allow you to divide up the parts of a page. The names of these elements indicate the kind of content you will find in them. They are still subject to change, but that has not stopped many web page authors using them already.
 
Headers & Footers header AND footer
 
 
Navigation | The nav element is used to contain the major navigational blocks on the site such as the primary site navigation.
        <nav>
        
        
Articles | The article element acts as a container for any section of a page that could stand alone and potentially be syndicated.
        <article>

Asides
         <aside>
         
The <aside> element has two
purposes, depending on whether
it is inside an <article>
element or not.
When the aside element
is used inside an article
element, it should contain
information that is related to the
article but not essential to its
overall meaning. For example, a
pullquote or glossary might be
considered as an aside to the
article it relates to.
When the <aside> element is
used outside of an <article>
element, it acts as a container
for content that is related to
the entire page. For example,
it might contain links to other
sections of the site, a list of
recent posts, a search box, or
recent tweets by the author.
  
  
        <section>
The <section> element groups
related content together, and
typically each section would
have its own heading.
For example, on a homepage
there may be several section
elements to contain different
sections of the page, such as
latest news, top products, and
newsletter signup
  
  
        <hgroup>
The purpose of the hgroup
element is to group together a
set of one or more h1 through
h6 elements so that they are
treated as one single heading.
  
        <figure> <figcaption>
You already met the figure
element in Chapter 5 when we
looked at images. It can be used
to contain any content that is
referenced from the main flow of
an article (not just images). 
  
  
 HTML5 allows web page authors
to place an <a> element around
a block level element that
contains child elements. This
allows you to turn an entire block
into a link.
This is not a new element in
HTML5, but it was not seen as a
correct usage of the a element
in earlier versions of HTML.
  
  
The new HTML5 elements indicate the purpose of
different parts of a web page and help to describe
its structure.
* The new elements provide clearer code (compared
with using multiple div elements).
* Older browsers that do not understand HTML5
elements need to be told which elements are
block-level elements.
* To make HTML5 elements work in Internet Explorer 8
(and older versions of IE), extra JavaScript is needed,
which is available free from Google.


Every website should be designed for the
target audience—not just for yourself or the
site owner. It is therefore very important to
understand who your target audience is


Target Audience: individuals
* What is the age range of your target audience?
* Will your site appeal to more women or men? What is the mix?
* Which country do your visitors live in?
* Do they live in urban or rural areas?
* What is the average income of visitors?
* What level of education do they have?
* What is their marital or family status?
* What is their occupation?
* How many hours do they work per week?
* How often do they use the web?
* What kind of device do they use to access the web?
Target Audience: Companies
* What is the size of the company or relevant department?
* What is the position of people in the company who visit your site?
* Will visitors be using the site for themselves or for someone else?
* How large is the budget they control?




Invent some fictional visitors from your typical
target audience. They will become your friends.
They can influence design decisions from color
palettes to level of detail in descriptions.


Now that you know who your visitors are, you
need to consider why they are coming. While
some people will simply chance across your
website, most will visit for a specific reason.


It is unlikely that you will be able to list every
reason why someone visits your site but you
are looking for key tasks and motivations. This
information can help guide your site designs.


You know who is coming to your site and why
they are coming, so now you need to work out
what information they need in order to achieve
their goals quickly and effectively.

Some sites benefit from being updated more
frequently than others. Some information (such
as news) may be constantly changing, while
other content remains relatively static.



Now that you know what needs to appear
on your site, you can start to organize the
information into sections or pages.

A wireframe is a simple sketch of the key
information that needs to go on each page of a
site. It shows the hierarchy of the information
and how much space it might require.


The primary aim of any kind of visual design
is to communicate. Organizing and prioritizing
information on a page helps users understand
its importance and what order to read it in.

Most web users do not read entire pages. Rather, they skim to find
information. You can use contrast to create a visual hierarchy that gets
across your key message and helps users find what they are looking for


Visual hierarchy refers to the order in which your eyes perceive what
they see. It is created by adding visual contrast between the items being
displayed. Items with higher contrast are recognized and processed first.


Images
Images create a high visual
contrast and often attract the
eye first. They can be used to
draw attention to a specific
message within the page. In
some cases, the right image can
succinctly reveal more than an
entire page of text

When making sense of a design, we tend to organize visual elements
into groups. Grouping related pieces of information together can make a
design easier to comprehend. Here are some ways this can be achieved.

We naturally observe similarities in design, and things that are similar are
perceived to be more related than things that are dissimilar. Repetition
of similar color, size, orientation, texture, font, or shape, suggests that
matching elements have similar importance or meaning

Site navigation not only helps people find where they want to go, but also
helps them understand what your site is about and how it is organized.
Good navigation tends to follow these principles...


* Concise
* Clear
* Selective
* Context
* Interactive
* Consistent



It's important to understand who your target audience
is, why they would come to your site, what information
they want to find and when they are likely to return.
* Site maps allow you to plan the structure of a site.
* Wireframes allow you to organize the information that
will need to go on each page.
* Design is about communication. Visual hierarchy helps
visitors understand what you are trying to tell them.
* You can differentiate between pieces of information
using size, color, and style.
* You can use grouping and similarity to help simplify
the information you present.




A script is a series of instructions that a
computer can follow to achieve a goal.
You could compare scripts to any of the following: 


To write a script, you need to first
state your goal and then list the
tasks that need to be completed in
order to achieve it. 


Start with the big picture of what
you want to achieve, and break
that down into smaller steps. 

1: DEFINE THE GOAL 
2: DESIGN THE SCRIPT 
3: CODE EACH STEP 

Every step for every task shown
in a flowchart needs to be written
in a language the computer can
understand and follow. 


You need to learn to "think" like
a computer because they solve
tasks in different ways than you or
I might approach them. 


Consider how you might approach a different type of script.
This example calculates the cost of a name plaque.
Customers are charged by the letter. 



Often scripts will need to perform different tasks in different situations.
You can use flowcharts to work out how the tasks fit together.
The flowcharts show the paths between each step. 

* A script is a series of instructions that the computer
can follow in order to achieve a goal.
* Each time the script runs, it might only use a subset of
all the instructions.
* Computers approach tasks in a different way than
humans, so your instructions must let the computer
solve the task prggrammatically.
* To approach writing a script, break down your goal into
a series of tasks and then work out each step needed
to complete that task (a flowchart can help). 



Here is a model of a hotel, along with some model trees, model people,
and model cars. To a human, it is clear what kind of real-world object
each one represents. 

If you could not see the picture of the hotel and cars, the data in the
information boxes alone would still tell you a lot about this scene. 

In the real world, people interact with objects. These interactions can
change the values of the properties in these objects. 


Methods represent things people need to do with objects. They can
retrieve or update the values of an object's properties. 

Computers use data to create models of things in the real world.
The events, methods, and properties of an object all relate to each other:
Events can trigger methods, and methods can retrieve or update an
object's properties. 


You have seen how data can be used to create a model of a hotel or a car.
Web browsers create similar models of the web page they are showing
and of the browser window that the page is being shown in. 


Using the document object, you can access and change what content
users see on the page and respond to how they interact with it. 


In order to understand how you can change the content of an HTML
page using JavaScript, you need to know how a browser interprets the
HTML code and applies styling to it


Before diving into the JavaScript language, you
need to know how it will fit together with the
HTML and CSS in your web pages. 




These three layers form the basis of a popular
approach to building web pages called
progressive enhancement. 

JavaScript is written in plain text, just like HTML and CSS, so you do not
need any new tools to write a script. This example adds a greeting into an
HTML page. The greeting changes depending on the time of day. 

When you want to use JavaScript with a web page, you use the HTML
script element to tell the browser it is coming across a script.
Its s re attribute tells people where the JavaScript file is stored. 
  
  
  
If you look at the source code for the example
you just created, you will see that the HTML is
still exactly the same. 


You may see JavaScript in the HTML between
opening script and closing script tags
(but it is better to put scripts in their own files).
  
  
It is best to keep JavaScript code in its own JavaScript
file. JavaScript files are text files (like HTML pages and
CSS style sheets), but they have the . j s extension.
The HTML script element is used in HTML pages
to tell the browser to load the JavaScript file (rather like
the <link> element can be used to load a CSS file).
If you view the source code of the page in the browser,
the JavaScript will not have changed the HTML,
because the script works with the model of the web
page that the browser has created. 











