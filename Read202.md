# Text tag in html

**HTML elements are used to describe the structure of
the page :**

1- Headings

2- Paragraphs

3- Bold & Italic

4- Superscript & Subscrip




**White Space**
When the browser comes across
two or more spaces next to each
other, it only displays one space.
Similarly if it comes across a line
break, it treats that as a single
space too. This is known as
white space collapsing.

**Semantic Markup**

its text elements that are not intended to affect the
structure of your web pages, but they do add extra information to the
pages like :

1- Quotations

2- Strong & Emphasis

3- Abbreviations & Acronyms

4- Author Details

5- Changes to Content


![taghtml](https://miro.medium.com/max/1276/1*EjUlBjd1yQFFcOvo0VYLog.jpeg)

# CSS

![css](https://ingzha.com/wp-content/uploads/2020/03/css-declaration-small.png)

CSS (Cascading Style Sheets) is a language for specifying how documents are presented to users, It is used to build web pages along with HTML. It has the advantage of adding features and properties to the structure of web pages, such as the colors, fonts, and styles that a web page takes.

**Three Ways to Insert CSS**

External CSS (preferred)
Internal CSS
Inline CSS+

**CSS Selectors**

There are many different types
of CSS selector that allow you to
target rules to specific elements
in an HTML document, for exp :
1- Class Selector
2- Universal Selector
3- ID Selector

and there are other types, you will find all types with an explanation by reference

[References](https://wtf.tw/ref/duckett.pdf) - page 238


**How Css Rules Cascade**

1- LAST RULE :
If the two selectors are identical,
the latter of the two will take
precedence

2- SPECIFICITY :
If one selector is more specific
than the others, the more
specific rule will take precedence
over more general ones

3- IMPORTANT :
You can add important after
any property value to indicate
that it should be considered
more important than other rules
that apply to the same element.

# JavaScript

**STATEMENTS**

A script is a series of instructions that a computer can follow one-by-one.
Each individual instruction or step is known as a statement. 

JAVASCRIPT IS CASE SENSITIVE
JavaScript is case sensitive so hourNow means
something different to HourNow or HOURNOW. 

**COMMENTS**

comments to explain what your code does.
They help make your code easier to read and understand. 

**variables**

A script will have to temporarily
store the bits of information it
needs to do its job. It can store this
data in variables. 

**DATA TYPES**

JavaScript distinguishes between numbers,
strings, and true or false values known as
Booleans. 

**ARRAYS**

An array is a special type of variable. It doesn't
just store one value; it stores a list of values. 

>var colors;

>colors ['white', 'black', ' custom'];

**OPERATORS**

Expressions rely on things called operators; they allow programmers to
create a single value from one or more values. 

**COMPARISON OPERATORS**
Compare two values and return true or false

>buy = 3 > 5;
The value of buy is false. 

**STRING OPERATORS**
>greeting= 'Hi 1 + 'Molly'; 

# Decision and looping

**DECISIONS**

A programming language uses control statements to control the flow of execution of program based on certain conditions. These  are used to cause the flow of execution to advance and branch based on changes to the state of a program.

**if**

![ifelse](https://media.geeksforgeeks.org/wp-content/uploads/nested-if-modified-1.png)

if: if statement is the most simple decision making statement. It is used to decide whether a certain statement or block of statements will be executed or not

>if(condition) 

   // Statements to execute if
   // condition is true

**if-else**

![ifelse](https://media.geeksforgeeks.org/wp-content/uploads/if-elseif.png)

Here, a user can decide among multiple options.The if statements are executed from the top down. As soon as one of the conditions controlling the if is true, the statement associated with that if is executed, and the rest of the ladder is bypassed. If none of the conditions is true, then the final else statement will be executed.

>if (condition)
    statement;
else if (condition)
    statement;
.
.
else
    statement;


[References](https://www.geeksforgeeks.org/decision-making-javaif-else-switch-break-continue-jump/)










