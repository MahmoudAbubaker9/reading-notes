# Layout

**Building Blocks**

CSS treats each HTML element as if it is in its
own box. This box will either be a block-level
box or an inline box.

1- Block-level elements

start on a new line
Examples include:
> h1 p ul li

2- Inline elements

flow in between
surrounding text
Examples include:
> img b i

**Containing Elements**

If one block-level element sits inside another
block-level element then the outer box is
known as the containing or parent element.

**Controlling the Position of Elements**

CSS has the following positioning schemes that allow you to control
the layout of a page: normal flow, relative positioning, and absolute
positioning. You specify the positioning scheme using the position
property in CSS. You can also float elements using the float property.

To indicate where a box should be positioned, you may also need to use
box offset properties to tell the browser how far from the top or bottom
and left or right it should be placed.

**Controlling the Position of Elements**

**Normal Flow**

position:static

In normal flow, each block-level
element sits on top of the next
one. Since this is the default
way in which browsers treat
HTML elements, you do not
need a CSS property to indicate
that elements should appear
in normal flow,

**Relative Positioning**

position:relative

Relative positioning moves an
element in relation to where it
would have been in normal flow

You then use the offset
properties (top or bottom and
left or right) to indicate how
far to move the element from
where it would have been in
normal flow.

**Absolute positioning**

position:absolute

When the position property
is given a value of absolute,
the box is taken out of normal
flow and no longer affects the
position of other elements on
the page

The box offset properties (top
or bottom and left or right)
specify where the element
should appear in relation to its
containing element.

**Fixed positioning**

position:Fixed

Fixed positioning is a type
of absolute positioning that
requires the position property
to have a value of fixed.

It positions the element in
relation to the browser window.
Therefore, when a user scrolls
down the page, it stays in the
exact same place. It is a good
idea to try this example in your
browser to see the effect.

**Overlapping Elements**

z-index

When you use relative, fixed, or
absolute positioning, boxes can
overlap. If boxes do overlap, the
elements that appear later in the
HTML code sit on top of those
that are earlier in the page.
If you want to control which
element sits on top, you can use
the z-index property. Its value
is a number, and the higher the
number the closer that element
is to the front. For example, an
element with a z-index of 10
will appear over the top of one
with a z-index of 5.

**Floating Elements**

The float property allows you
to take an element in normal
flow and place it as far to the
left or right of the containing
element as possible.
Anything else that sits inside
the containing element will
flow around the element that is
floated.

**Clearing Floating**
The clear property allows you
to say that no element (within
the same containing element)
should touch the left or righthand sides of a box. 


If a containing element only
contains floated elements, some
browsers will treat it as if it is
zero pixels tall.

**Page Sizes**

Because screen sizes and display resolutions vary so much, web
designers often try to create pages of around 960-1000 pixels wide
(since most users will be able to see designs this wide on their screens).

## Type of Layouts

1- Fixed Width Layouts

Fixed width layout
designs do not
change size as the
user increases
or decreases
the size of their
browser window.
Measurements tend
to be given in pixels.

2- Liquid Layouts

Liquid layout designs
stretch and contract
as the user increases
or decreases the
size of their browser
window. They tend to
use percentages


* Grids help create professional and flexible designs.
* CSS Frameworks provide rules for common tasks.
* You can include multiple CSS files in one page.
