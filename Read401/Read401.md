# Java Basics

## Language Basics

**1- Variables :**

The term variable is used in the Java language and its types are:

1- Instance Variables (Non-Static Fields) 

Non static fields are also known as instance variables because their values are unique to each instance of a class (for each object)

2- Class Variables (Static Fields)

if a field is declared static, then exactly a single copy of that field is created and shared among all instances of that class. It doesn't matter how many times we initialize a class; there will always be only one copy of static field belonging to it. 


3- Local Variables

 a method will often store its temporary state in local variables. The syntax for declaring a local variable is similar to declaring a field (for example, int count = 0;). There is no special keyword designating a variable as local

4- Parameters

 in the main method (public static void main(String[] args). Here the args variable is the parameter to this method



**2-Operators:**

Operators in Java have precedence which means a certain operator is priorities in execution over another operator

![Operators](https://www.softwaretestingmaterial.com/wp-content/uploads/2018/03/Operators-Table.png)

**3-Expressions, Statements, and Blocks:**

Expressions : a construct that use operators, variables, and method invocations, an expression returns Boolean data

Statements : a complete unit of execution and is terminated by semicolon ;

block : is a group of zero or more statements between balanced braces and can be used anywhere a single statement is allowed.

**4- Control Flow Statements:**

![Control Flow](https://camo.githubusercontent.com/2b102bd44d3f2963b52e0656832428c9929d32c022cccedac7d12f080366de20/68747470733a2f2f312e62702e626c6f6773706f742e636f6d2f2d43505945657875643462592f5862674f71435f505064492f4141414141414141444b672f6937584a5f78714559464d5f37597730655a713664466844617562317330632d67434c63424741735948512f73313630302f6a6176612d636f6e74726f6c2d666c6f772d73746174656d656e742e706e67)


The statements inside your source files are generally executed from top to bottom, in the order that they appear. Control flow statements, This section describes:

1- Decision making statements : if-then , if-then-else, switch

2- Looping statements : for , while, do-while

3- Branching statements : break , continue , return


**compile code**

![compile](https://imgs.xkcd.com/comics/compiling.png)

the compiler (usually another program) takes the program the human wrote, and converts it into the program the computer can understand like converts from Java to machine language.

The very short version could be, yes, compile means to make the code executable.