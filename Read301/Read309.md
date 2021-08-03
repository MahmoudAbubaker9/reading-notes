# FUNCTIONAL PROGRAMMING

## Functional Programming Concepts

## 1. What is functional programming?

Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data

## 2. What is a pure function and how do we know if something is a pure function?

(a block of code ) that always returns the same result if the same arguments are passed. It does not depend on any state, or data change during a program's execution rather it only depends on its input arguments

### So how do we know if a function is pure or not?

1. It returns the same result if given the same arguments (it is also referred as deterministic)

2. It does not cause any observable side effects

## 3. What are the benefits of a pure function?

The code’s definitely easier to test. We don’t need to mock anything.

## 4. What is immutability?

When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.


## 5. What is Referential transparency?

Basically, if a function consistently yields the same result for the same input, it is referentially transparent.

>pure functions + immutable data = referential transparency

With this concept, a cool thing we can do is to memoize the function. Imagine we have this function:

>const sum = (a, b) => a + b;


# Node JS Tutorial for Beginners #6 - Modules and require()

## 1. What is a module?

Just another JavaScript file that does a certain functionality of the code.

## 2. What does the word ‘require’ do?

The require function is intended to add separate pieces of code (“modules”) to the current scope.

## 3. How do we bring another module into the file the we are working in?

by export it then require it in the needed file.

## 4. What do we have to do to make a module available?

Export it using module.exports.