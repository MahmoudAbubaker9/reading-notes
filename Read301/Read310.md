# In memory storage

## Understanding the JavaScript Call Stack

## 1. What is a ‘call’?

The call stack is primarily used for function invocation (call). 

## 2. How many ‘calls’ can happen at once?

Since the call stack is single, function(s) execution, is done one at a time, from top to bottom. It means the call stack is synchronous.

## 3. What does LIFO mean?

When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

## 4. Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

function firstFunction(){
  console.log("Hello from firstFunction");
}

function secondFunction(){
  firstFunction();
  console.log("The end from secondFunction");
}

secondFunction();

![call stack](https://cdn-media-1.freecodecamp.org/images/oEp65Ec9CD4CnL7t0uSPoyzrkA1i1BR-Ij1n)

## 5. What causes a Stack Overflow?

A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.

## This is what happens when the code is run:

1. When secondFunction() gets executed, an empty stack frame is created. It is the main (anonymous) entry point of the program.
2. secondFunction() then calls firstFunction()which is pushed into the stack.
3. firstFunction() returns and prints “Hello from firstFunction” to the console.
4. firstFunction() is pop off the stack.
5. The execution order then move to secondFunction().
6. secondFunction() returns and print “The end from secondFunction” to the console.
7. secondFunction() is pop off the stack, clearing the memory.


# JavaScript error messages

## 1. What is a ‘refrence error’?

This is as simple as when you try to use a variable that is not yet declared you get this type os errors.

>console.log(foo) // Uncaught ReferenceError: foo is not defined

## 2. What is a ‘syntax error’?

this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.


## 3. What is a ‘range error’?

Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.


## 4. What is a ‘type error’?

this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.


## 5. What is a breakpoint?

It is used when debugging, it stops the compiler at a certain line, giving the values for all the variables, in order to fix a bug in the application.

## 6. What does the word ‘debugger’ do in your code?

A debugger is a software tool that can help the software development process by identifying coding errors at various stages of the operating system or application development. Some debuggers will analyze a test run to see what lines of code were not executed.

