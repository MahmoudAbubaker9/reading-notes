# Images

There are several things to consider when selecting and
preparing images for your site, but taking time to get them
right will make it look more attractive and professional.
In this chapter you will learn how to:

● Include an image in your web pages using HTML

● Pick which image format to use

● Show an image at the right size

● Optimize an image for use on the web to make pages
load faster

**If you are building a site from scratch, it is good
practice to create a folder for all of the images
the site uses.**

**Three Rules for Creating Images**

1-Save images in the right format

2-Save images at the right size

3-Use the correct resolution

**Image Dimensions**

The images you use on your website should be
saved at the same width and height that you
want them to appear on the page

**Cropping Images**

When cropping images it is important not to
lose valuable information. It is best to source
images that are the correct shape if possible

# Color

The color property allows you
to specify the color of text inside
an element. You can specify any
color in CSS in one of three ways:

1- rgb values : Values for red, green, and blue
are expressed as numbers
between 0 and 255.

2- hex codes : Hex values represent values
for red, green, and blue in
hexadecimal code. *hsl, hsla*

3- color names : Colors are represented by
predefined names. However,
they are very limited in number.There are 147 color names



**opacity :

CSS3 introduces the opacity
property which allows you to
specify the opacity of an element
and any of its child elements.
The value is a number between
0.0 and 1.0 (so a value of 0.5
is 50% opacity and 0.15 is 15%
opacity).**

# Text

The properties that allow you to control
the appearance of text can be split into
two groups:

● Those that directly affect the font and its appearance
(including the typeface, whether it is regular, bold or italic,
and the size of the text)

● Those that would have the same effect on text no matter
what font you were using (including the color of text and
the spacing between words and letters)

**Specifying Typefaces**

1- font-family

The font-family property
allows you to specify the
typeface that should be used for
any text inside the element(s) to
which a CSS rule applies.


2- font-size

The font-size property enables
you to specify a size for the
font

3- font-face

font-face allows you to use
a font, even if it is not installed
on the computer of the person
browsing, by allowing you to
specify a path to a copy of the
font, which will be downloaded if
it is not on the user's machine.

>@font-face {

>font-family: 'ChunkFiveRegular';

>src: url('fonts/chunkfive.eot');}

4- font-weight

The font-weight property
allows you to create bold text.
There are two values that this
property commonly takes:

-normal

This causes text to appear at a
normal weight.

-bold

This causes text to appear bold.

5- font-style

-normal

This causes text to appear in a
normal style (as opposed to italic
or oblique).

-italic

This causes text to appear italic.

-oblique

This causes text to appear
oblique.

6- UpperCase & LowerCase

7- Underline & Strike 

8- Leading (line-height)

Leading (pronounced ledding) is
a term typographers use for the
vertical space between lines of
text

9- letter-spacing, word-spacing

10- text-align and vertical-align

11- text-indent

12- text-shadow

13- :first-letter, :first-line

14- :hover, :active, :focus




[Attribute Selectors Ref. - Page 292](https://wtf.tw/ref/duckett.pdf)

# JPEG vs PNG vs GIF

**JPEG**

images don’t support transparency and are hence not usable for such cases and can support around 16 million colours. This is what makes them suitable for storing images of natural scenes.

**PNG**

images mainly have two modes — PNG8 and PNG24. PNG8 can support upto 256 colours whereas PNG24 can handle upto 16 million colours like a JPEG imagea and mages support transparency in two ways.


**GIF**

images support transparency by declaring a single colour in the colour palette as transparent (index transparency) and GIF images are limited to 256 colours

