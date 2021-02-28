
## Chapter 2: “Text” (pp.40-61)

When creating a web page, you add tags
(known as markup) to the contents of the
page. These tags provide extra meaning
and allow browsers to show users the
appropriate structure for the page.


*  Structural markup: the elements that you can use to
describe both headings and paragraphs
* Semantic markup: which provides extra information; such
as where emphasis is placed in a sentence, that something
you have written is a quotation (and who said it), the
meaning of acronyms, and so on


### HTML has six "levels" of headings:

h1 is used for main headings
h2 is used for subheadings
If there are further sections
under the subheadings then the
h3 element is used, and so
on...



        <p>
To create a paragraph, surround
the words that make up the
paragraph with an opening p
tag and closing /p tag.


      <b>
By enclosing words in the tags
b and /b we can make
characters appear bold.



      <i>
By enclosing words in the tags
i and /i we can make
characters appear italic.


      <sup>
The sup element is used
to contain characters that
should be superscript such
as the suffixes of dates or
mathematical concepts like
raising a number to a power such
as 22.

        <sub>
The sub element is used to
contain characters that should
be subscript. It is commonly
used with foot notes or chemical
formulas such as H2.
  
  
  
  When the browser comes across
two or more spaces next to each
other, it only displays one space.
Similarly if it comes across a line
break, it treats that as a single
space too. This is known as
white space collapsing.



        <br />
As you have already seen, the
browser will automatically show
each new paragraph or heading
on a new line. But if you wanted
to add a line break inside the
middle of a paragraph you can
use the line break tag br /.



       <hr />
To create a break between
themes — such as a change of
topic in a book or a new scene
in a play — you can add a
horizontal rule between sections
using the hr / tag.

<hr>
<hr>
<hr>


Content management systems and HTML editors such as Dreamweaver
usually have two views of the page you are creating: a visual editor and a
code view.


There are some text elements that are not intended to affect the
structure of your web pages, but they do add extra information to the
pages — they are known as semantic markup.




        <strong>
The use of the strong
element indicates that its
content has strong importance.
For example, the words
contained in this element might
be said with strong emphasis.


      <em>
The em element indicates
emphasis that subtly changes
the meaning of a sentence.


      <blockquote>
The blockquote element is
used for longer quotes that take
up an entire paragraph. Note
how the <p> element is still
used inside the blockquote
element. 
  
  
  
    <q>
The q element is used for
shorter quotes that sit within
a paragraph. Browsers are
supposed to put quotes around
the q element, however
Internet Explorer does not —
therefore many people avoid
using the q element.


      <abbr> 
If you use an abbreviation or
an acronym, then the abbr
element can be used. A title
attribute on the opening tag is
used to specify the full term.



      <cite>
When you are referencing a
piece of work such as a book,
film or research paper, the
cite element can be used
to indicate where the citation is
from.


    <dfn>
The first time you explain some
new terminology (perhaps an
academic concept or some
jargon) in a document, it is
known as the defining instance
of it.


    <address> 
The address element has
quite a specific use: to contain
contact details for the author of
the page.

    <ins>
    <del>
The ins element can be used
to show content that has been
inserted into a document, while
the del element can show text
that has been deleted from it
  
     <s>
The s element indicates
something that is no longer
accurate or relevant (but that
should not be deleted).


HTML elements are used to describe the structure of
the page (e.g. headings, subheadings, paragraphs).
X They also provide semantic information (e.g. where
emphasis should be placed, the definition of any
acronyms used, when given text is a quotation).



<hr>

<hr>

<hr>
## Chapter 10: Ch.10 “Introducing CSS” (pp.226-245)

The key to understanding how CSS works is to
imagine that there is an invisible box around
every HTML element.


CSS works by associating rules with HTML elements. These rules govern
how the content of specified elements should be displayed. A CSS rule
contains two parts: a selector and a declaration

CSS declarations sit inside curly brackets and each is made up of two
parts: a property and a value, separated by a colon. You can specify
several properties in one declaration, each separated by a semi-colon.


      <link> 
The link element can be used
in an HTML document to tell the
browser where to find the CSS
file used to style the page. It is an
empty element (meaning it does
not need a closing tag), and it
lives inside the head element.
It should use three attributes:

1. href
2. type
3. rel


        <style>
You can also include CSS rules
within an HTML page by placing
them inside a style element,
which usually sits inside the
head element of the page.


![css selectors](https://i.ibb.co/ydTnH2d/validatorhtml.png)


###### LAST RULE
If the two selectors are identical,
the latter of the two will take
precedence. Here you can see
the second i selector takes
precedence over the first.

###### SPECIFICITY
If one selector is more specific
than the others, the more
specific rule will take precedence
over more general ones. 


###### IMPORTANT
You can add !important after
any property value to indicate
that it should be considered
more important than other rules
that apply to the same element

<hr>

<hr>

<hr>


#### When building a website there are several advantages to placing your CSS rules in a separate style sheet.


CSS1 was released in 1996 and CSS2 followed two years later. Work on
CSS3 has been ongoing but the major browsers have already started to
implement it.

Any seasoned user of CSS will tell you that some browsers display a few
of the CSS properties in an unexpected way. But finding and squashing
those bugs is easy when you know how...


CSS treats each HTML element as if it appears inside
its own box and uses rules to indicate how that
element should look.


* Rules are made up of selectors (that specify the
elements the rule applies to) and declarations (that
indicate what these elements should look like).
* Different types of selectors allow you to target your
rules at different elements.
* Declarations are made up of two parts: the properties
of the element that you want to change, and the values
of those properties. For example, the font-family
property sets the choice of font, and the value arial
specifies Arial as the preferred typeface.
* CSS rules usually appear in a separate document,
although they may appear within an HTML page.



<hr>
<hr>
<hr>



