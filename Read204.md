# Links

Links are the defining feature of the web
because they allow you to move from
one web page to another

> < a href="site link">name</ a>

types of links:
1-Linking to Other Sites
2- Linking to Other Pages on the Same Site

**Relative URLs Type**
1-Parent Folder
2- Child Folder
3-Grandchild Folder

**Email Links**
the value of the href attribute starts
with mailto: and is followed by
the email address you want the
email to be sent to

> < a href="@example.org">Email < /a>

**Opening Links in a New Window**

> < a href="site name" target="_blank" >

# Layout

**Block**

Building Blocks :

CSS treats each HTML element as if it is in its
own box. This box will either be a block-level
box or an inline box

Containing Elements :

If one block-level element sits inside another
block-level element then the outer box is
known as the containing or parent element.

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

# Functions, Methods, and Objects

Functions let you group a series of statements together to perform a
specific task. If different parts of a script repeat the same task, you can
reuse the function (rather than repeating the same set of st atements).

>Example
function myFunction(p1, p2) {
  return p1 * p2;   
}
>// The function returns the product of p1 and p2

**Function Invocation**

When an event occurs (when a user clicks a button)
When it is invoked (called) from JavaScript code
Automatically (self invoked)

**Function Return**
When JavaScript reaches a return statement, the function will stop executing.

Functions Used as Variable Values
Functions can be used the same way as you use variables, in all types of formulas, assignments, and calculations

**Function declarations**

A function definition (also called a function declaration, or function statement) consists of the function keyword, followed by:

The name of the function.
A list of parameters to the function, enclosed in parentheses and separated by commas.
The JavaScript statements that define the function, enclosed in curly brackets, {...}.

**VARIABLE SCOPE**

The location where you declare a variable will affect where it can be used
within your code. If you declare it within a function, it can only be used
within that function. This is known as the variable's scope

1- LOCAL VARIABLES

When a variable is created inside a function using the
var keyword, it can only be used in that function.
It is called a local variable or function-level variable.
It is said to have local scope or function-level scope.
It cannot be accessed outside of the function in
which it was declared

2- GLOBAL VARIABLES 

If you create a variable outside of a function, then it
can be used anywhere within the script. It is called a
global variable and has global scope.

**HOW MEMORY & VARIABLES WORK**

Global variables use more memory. The browser has to remember them
for as long as the web page using them is loaded. Local variables are only
remembered during the period of time that a function is being executed

# Pair Programming

While learning to code, developers likely study several programming languages. Similar to a foreign language class, there are four fundamental skills that help anyone learn a new language: Listening: hearing and interpreting the vocabulary Speaking: using the correct words to communicate an idea Reading: understanding what written language intends to convey Writing: producing from scratch a meaningful

1- Greater efficiency

It is a common misconception that pair programming takes a lot longer and is less efficient. In reality, when two people focus on the same code base, it is easier to catch mistakes in the making.


2- Engaged collaboration

When two programmers focus on the same code, the experience is more engaging and both programmers are more focused than if they were working alone. It is harder to procrastinate or get off track when someone else is relying on you to complete the work.

3- Learning from fellow students

Everyone has a different approach to problem solving; working with a teammate can expose developers to techniques they otherwise would not have thought of. 

4- Social skills

Pair programming is great for improving social skills. When working with someone who has a different coding style, communication is key. This can become more difficult when two programmers have different personalities. Pair programming not only improves programming skills, but can also help programmers develop their interpersonal skills. 

5- Job interview readiness

A common step in many interview processes involves pair programming between a current employee and an applicant, either in person or through a shared screen. They will carry out exercises together, such as code challenges, building a project or feature, or debugging an existing code base. By doing so, companies can get a better feel for how an applicant will fit into the team and their collaboration style.

6- Work environment readiness

Many companies that utilize pair programing expect to train fresh hires from CS-degree programs on how they operate to actually deliver a product. Code Fellows graduates who are already familiar with how pairing works can hit the ground running at a new job, with one less hurdle to overcome.