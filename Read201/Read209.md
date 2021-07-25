# Forms

Traditionally, the term 'form' has referred
to a printed document that contains
spaces for you to fill in information.

HTML borrows the concept of a form to refer to different
elements that allow you to collect information from visitors to
your site.

**Form Controls**

There are several types of form controls that
you can use to collect information from visitors
to your site.

1- ADDING TEXT

2- Making Choices

3- Submitting Forms

**Form Structure**

1- action
Every form element requires
an action attribute. Its value
is the URL for the page on the
server that will receive the
information in the form when it
is submitted

2- method
Forms can be sent using one of
two methods: get or post.
With the get method, the values
from the form are added to
the end of the URL specified in
the action attribute. T

**-Input types**


1- Text input

2- Password Input

3- Text area

4- Radio Button

5- Checkbox

6- Drop Down List Box

7- Multiple select box

8- File Input Box

9- img + Submit button

10 - Button & hidden Controls


# Lists, Tables and Forms

There are several CSS properties that
were created to work with specific types
of HTML elements, such as lists, tables,
and forms.

- In addition to the CSS properties covered in other
chapters which work with the contents of all elements,
there are several others that are specifically used to
control the appearance of lists, tables, and forms.

- List markers can be given different appearances
using the list-style-type and list-style image
properties.

- Table cells can have different borders and spacing in
different browsers, but there are properties you can
use to control them and make them more consistent.

- Forms are easier to use if the form controls are
vertically aligned using CSS.

- Forms benefit from styles that make them feel more
interactive.

# Events

An HTML event can be something the browser does, or something a user does.

Here are some examples of HTML events:

An HTML web page has finished loading

An HTML input field was changed

An HTML button was clicked

element .addEventlistener('event', functionName [, Boolean]) ;

**THREE WAYS TO BIND AN EVENT TO AN ELEMENT**

1- HTML EVENT HANDLERS

2- TRADITIONAL DOM  EVENT HANDLERS :

All modern browsers understand this way of creating an event handler,
but you can only attach one function to each event handler.

element.onevent = functionName ;

3- DOM LEVEL 2 EVENT LISTENERS

**EVENT LISTENERS**

Event listeners are a more recent approach to handling events.
They can deal with more than one function at a time
but they are not supported in older browsers.

element .addEventlistener('event', functionName [, Boolean]) ;


**THE EVENT OBJECT**

When an event occurs, the event object tells
you information about the event, and the
element it happened upon.

the The event object is passed to
any function that is the event
handler or listener.

Creating event listeners for a lot of elements
can slow down a page, but event flow allows
you to listen for an event on a parent element.
 

**CHANGING DEFAULT BEHAVIOR**

The event object has methods that change:
the default behavior of an element and how
the element's ancestors respond to the event.

1- preventDefault ()

Some events, such as clicking on
links and submitting forms, take
the user to another page.
To prevent the default behavior
of such elements (e.g., to keep
the user on the same page
rather than following a link
or being taken to a new page
after submitting a form), you
can use the event object's
preventoefault() method.

2- stopPropagation()

Once you have handled an
event using one element, you
may want to stop that event
from bubbling up to its ancestor
elements (especially if there
are separate event handlers
responding to the same events
on the containing elements).
To stop the event bubbling up,
you can use the event object's
stopPropogation() method.

**WHICH ELEMENT DID AN EVENT OCCUR ON?**

When calling a function, the event object's target property is the best
way to determine which element the event occurred on. But you may see
the approach below used; it relies on the this keyword.

**DIFFERENT TYPES OF EVENTS**

1- USER INTERFACE EVENTS

User interface CUI) events occur as a result of interaction with the
browser window rather than the HTML page contained within it,
e.g., a page having loaded or the browser window being resized.

* Ref at 272 Page

2- FOCUS & BLUR EVENTS

The HTML elements you can interact with, such as links and form
elements, can gain focus. These events fire when they gain or lose focus.

3- MOUSE EVENTS

The mouse events are fired when the mouse is moved and also when its
buttons are clicked.

4- KEYBOARD EVENTS

The keyboard events are fired when a user interacts with the keyboard
(they fire on any kind of device with a keyboard).

5- FORM EVENTS

There are two events that are commonly used with forms.
In particular you are likely to see submit used in form validation. (submit,change,input)

6- MUTATION EVENTS & OBSERVERS

Whenever elements are added to or removed from the DOM, its
structure changes. This change triggers a mutation event.


* The most commonly used events are W3C DOM
events, although there are others in the HTMLS
specification as well as browser-specific events.

* When an event occurs on an element, it can trigger a
JavaScript function. When this function then changes
the web page in some way, it feels interactive because
it has responded to the user.