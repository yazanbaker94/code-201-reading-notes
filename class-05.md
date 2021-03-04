There are many reasons why you might
want to add an image to a web page: you
might want to include a logo, photograph,
illustration, diagram, or chart.


A picture can say a thousand words, and great
images help make the difference between an
average-looking site and a really engaging one.


If you are building a site from scratch, it is good
practice to create a folder for all of the images
the site uses

	img

To add an image into the page
you need to use an img
element. This is an empty
element (which means there is
no closing tag). It must carry the
following two attributes:

	src
This tells the browser where
it can find the image file. This
will usually be a relative URL
pointing to an image on your
own site. 


	title
You can also use the title
attribute with the img element
to provide additional information
about the image. Most browsers
will display the content of this
attribute in a tootip when the
user hovers over the image.


	height
This specifies the height of the
image in pixels.

	width
This specifies the width of the
image in pixels.




	align
The align attribute was
commonly used to indicate how
the other parts of a page should
flow around an image. It has
been removed from HTML5
and new websites should use
CSS to control the alignment of
images.



	left
This aligns the image to the left
(allowing text to flow around its
right-hand side).


	right
This aligns the image to the right
(allowing text to flow around its
left-hand side).



	top
This aligns the first line of the
surrounding text with the top of
the image



	middle
This aligns the first line of the
surrounding text with the middle
of the image.

	bottom
This aligns the first line of the
surrounding text with the bottom
of the image.




There are three rules to remember when you
are creating images for your website which are
summarized below. We go into greater detail
on each topic over the next nine pages


1. Save images inthe right format
2. Save images atthe right size
3. Use the correct
resolution



There are several tools you can use to edit and
save images to ensure that they are the right
size, format, and resolution



The images you use on your website should be
saved at the same width and height that you
want them to appear on the page.



When cropping images it is important not to
lose valuable information. It is best to source
images that are the correct shape if possible.



Images created for the web should be saved at
a resolution of 72 ppi. The higher the resolution
of the image, the larger the size of the file.



Vector images differ from bitmap images and
are resolution-independent. Vector images are
commonly created in programs such as Adobe
Illustrator


Animated GIFs show several frames of an
image in sequence and therefore can be used to
create simple animations.




Creating an image that is partially transparent
(or "see-through") for the web involves
selecting one of two formats:


1. Transparent GIF
2. PNG


Checking the Size of Images
If you are updating a website, you might need to check the size of an
existing image before creating a new one to replace it. This can be
achieved by right-clicking on the image and making a selection from
the pop-up menu that appears. (Mac users will need to hold down the
control key and click rather than right-click.)



	figure
Images often come with
captions. HTML5 has introduced
a new figure element to
contain images and their caption
so that the two are associated.
You can have more than one
image inside the <figure>
element as long as they all share
the same caption.



	figcaption
The figcaption element has
been added to HTML5 in order
to allow web page authors to add
a caption to an image.


* The img element is used to add images to a
web page.
* You must always specify a src attribute to indicate the
source of an image and an alt attribute to describe the
content of an image.
* You should save images at the size you will be using
them on the web page and in the appropriate format.
* Photographs are best saved as JPEGs; illustrations or
logos that use flat colors are better saved as GIFs.



# Color can really bring your pages to life.


1. rgb values
2. hex codes
3. color names


background-color


Every color on a computer screen is created by mixing amounts of red,
green, and blue. To find the color you want, you can use a color picker.


* Hue
* Saturation
* Brightness



When picking foreground and background
colors, it is important to ensure that there is
enough contrast for the text to be legible.



CSS3 introduces an entirely new and intuitive
way to specify colors using hue, saturation,
and lightness values.


* Color not only brings your site to life, but also helps
convey the mood and evokes reactions.
* There are three ways to specify colors in CSS:
RGB values, hex codes, and color names.
* Color pickers can help you find the color you want.
* It is important to ensure that there is enough contrast
between any text and the background color (otherwise
people will not be able to read your content).
* CSS3 has introduced an extra value for RGB colors to
indicate opacity. It is known as RGBA.
* CSS3 also allows you to specify colors as HSL values,
with an optional opacity value. It is known as HSLA.



# Typeface Terminology


1. Serif
2. Sans-Serif
3. Monospace
4. Weight
5. Style 
6. Stretch


When choosing
a typeface, it
is important to
understand that a
browser will usually
only display it if it's
installed on that
user's computer.

1. Monospace
2. Cursive
3. Fantasy


There are several ways to use fonts other than those listed on the
previous page. However, typefaces are subject to copyright, so the
techniques you can choose from are limited by their respective licenses.



If you design on a Mac, it is important to check what the typefaces look
like on a PC because PCs can render type less smoothly. But if you design
on a PC, then it should look fine on a Mac.


The font-family property
allows you to specify the
typeface that should be used for
any text inside the element(s) to
which a CSS rule applies.


The font-size property enables
you to specify a size for the
font. There are several ways to
specify the size of a font. The
most common are:

1. pixels

2. percentages

3. ems



You may have noticed that programs such as
Word, Photoshop and InDesign offer the same
sizes of text.



@font-face allows you to use
a font, even if it is not installed
on the computer of the person
browsing, by allowing you to
specify a path to a copy of the
font, which will be downloaded if
it is not on the user's machine.


1. font-family
2. src
3. format

Different browsers support
different formats for fonts
(in the same way that they
support different audio and
video formats), so you will need
to supply the font in several
variations to reach all browsers.


The font-weight property
allows you to create bold text.
There are two values that this
property commonly takes:

1. normal
2. bold



If you want to create italic text,
you can use the font-style
property. There are three values
this property can take:


1. normal
2. italic
3. oblique



## text-transform
1. uppercase
2. lowercase
3. capitalize

## text-decoration

1. none
2. underline
3. overline
4. line-through
5. blink


## line-height


## letter-spacing, word-spacing 

Kerning is the term
typographers use for the space
between each letter. You can
control the space between each
letter with the letter-spacing
property.



## text-align
1. left
2. right
3. center
4. justify


## vertical-align
The vertical-align property is
a common source of confusion.
It is not intended to allow you to
vertically align text in the middle
of block level elements such as
<p> and <div>, although it does
have this effect when used with
table cells (the td and th
elements).

## text-indent

The text-indent property
allows you to indent the first
line of text within an element.
The amount you want the line
indented by can be specified in
a number of ways but is usually
given in pixels or ems.


## text-shadow

The text-shadow property has
become commonly used despite
lacking support in all browsers.



## :first-letter, :first-line

You can specify different values
for the first letter or first line of
text inside an element using
:first-letter and
:first-line. 


## :link, :visited


Browsers tend to show links
in blue with an underline by
default, and they will change
the color of links that have been
visited to help users know which
pages they have been to


## :hover, :active, :focus

1. :hover
2. :active
3. :focus



### TL;DR
"Use JPEG format for all images that contain a natural scene or photograph where variation in colour and intensity is smooth. Use PNG format for any image that needs transparency or for images with text & objects with sharp contrast edges like logos. Use GIF format for images that contain animations."


BOOKS/LINKS USED:

HTML AND CSS - DUCKETT

https://blog.imagekit.io/jpeg-vs-png-vs-gif-which-image-format-to-use-and-when-c8913ae3e01d
