### Centering images Using CSS


By default, images are inline
elements. This means that they
flow within the surrounding text.
In order to center an image, it
should be turned into a blocklevel element using the display
property with a value of block. 


background-image

The background-image
property allows you to place
an image behind any HTML
element. This could be the entire
page or just part of the page. By
default, a background image will
repeat to fill the entire box.


background-repeat
background-attachment


	repeat

The background image is
repeated both horizontally and
vertically (the default way it
is shown if the backgroundrepeat property isn't used).

	
	repeat-x

The image is repeated
horizontally only (as shown in
the first example on the left).

	repeat-y

The image is repeated vertically
only.


	no-repeat


	The background-attachment
property specifies whether a
background image should stay in
one position or move as the user
scrolls up and down the page. It
can have one of two values:


	fixed

The background image stays in
the same position on the page.

	scroll
The background image moves

up and down as the user scrolls
up and down the page.


	background-position

When an image is not being
repeated, you can use the
background-position
property to specify where in the
browser window the background
image should be placed


	background

The background property acts
like a shorthand for all of the
other background properties
you have just seen, and also the
background-color property.


Using CSS, it is possible to create
a link or button that changes to a
second style when a user moves
their mouse over it (known as a
rollover) and a third style when
they click on it. 


Gradients


CSS3 is going to introduce the
ability to specify a gradient for
the background of a box. The
gradient is created using the
background-image property
and, at the time of writing,
different browsers required a
different syntax.



If you want to overlay text on a background image, the image must be low
contrast in order for the text to be legible.



You can specify the dimensions of images using CSS.
This is very helpful when you use the same sized
images on several pages of your site.

* Images can be aligned both horizontally and vertically
using CSS.
* You can use a background image behind the box
created by any element on a page.
* Background images can appear just once or be
repeated across the background of the box.
* You can create image rollover effects by moving the
background position of an image.
* To reduce the number of images your browser has to
load, you can create image sprites.



Search Engine
Optimization (SEO)


SEO is a huge topic and several books have been written on the subject.
The following pages will help you understand the key concepts so you can
improve your website's visibility on search engines.



On-Page SEO

In every page of your website there are seven key places where keywords
(the words people might search on to find your site) can appear in order
to improve its findability.


Determining which keywords to use on your site can be one of the
hardest tasks when you start to think about SEO. Here are six steps that
will help you identify the right keywords and phrases for your site.



1: Brainstorm
2: Organize
3: Research
4: Compare
5: Refine
6: Map


As soon as people start coming to your site, you can start analyzing
how they found it, what they were looking at and at what point they are
leaving. One of the best tools for doing this is a free service offered by
Google called Google Analytics.


The overview page gives you a snapshot of the key information you are
likely to want to know. In particular, it tells you how many people are
coming to your site



The content link on the left-hand side allows
you to learn more about what the visitors are
looking at when they come to your site.



The traffic sources link on the left hand side
allows you to learn where your visitors are
coming from.




In order to put your site on the web you will
need a domain name and web hosting.


To transfer your code and images from your
computer to your hosting company, you use
something known as File Transfer Protocol.



There are a wide variety of sites that offer
services commonly created by web developers
(to save you having to build them yourself).




Search engine optimization helps visitors find your
sites when using search engines.

* Analytics tools such as Google Analytics allow you to
see how many people visit your site, how they find it,
and what they do when they get there.
*  To put your site on the web, you will need to obtain a
domain name and web hosting.
*  FTP programs allow you to transfer files from your
local computer to your web server.
*  Many companies provide platforms for blogging, email
newsletters, e-commerce and other popular website
tools (to save you writing them from scratch).



HTML5 video and audio

The video and audio elements allow us to embed video and audio into web pages. As we showed in Video and audio content, a typical implementation looks like this:


	<video controls>
	<source src="rabbit320.mp4" type="video/mp4">
	<source src="rabbit320.webm" type="video/webm">
	<p>Your browser doesn't support HTML5 video. Here is a <a href="rabbit320.mp4">link to the video</a> instead.</p>
	</video>



Part of the HTML5 spec, the HTMLMediaElement API provides features to allow you to control video and audio players programmatically — for example HTMLMediaElement.play(), HTMLMediaElement.pause(), etc. This interface is available to both <audio> and <video> elements, as the features you'll want to implement are nearly identical. Let's go through an example, adding features as we go.





Playing and pausing the video
Let's implement probably the most important control — the play/pause button.

First of all, add the following to the bottom of your code, so that the playPauseMedia() function is invoked when the play button is clicked:


	play.addEventListener('click', playPauseMedia);


Now to define playPauseMedia() — add the following, again at the bottom of your code:

	function playPauseMedia() {
	if(media.paused) {
	play.setAttribute('data-icon','u');
	media.play();
	} else {
	play.setAttribute('data-icon','P');
	media.pause();
	}
	}





Updating the elapsed time
The very last piece of our media player to implement is the time elapsed displays. To do this we'll run a function to update the time displays every time the timeupdate event is fired on the <video> element. The frequency with which this event fires depends on your browser, CPU power, et




LINKS/BOOKS USED:

1. https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Video_and_audio_APIs#html5_video_and_audio
2. HTML & CSS - DUCKETT
