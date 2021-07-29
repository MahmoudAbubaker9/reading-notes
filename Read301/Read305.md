# Thinking in React

React is, in our opinion, the premier way to build big, fast Web apps with JavaScript. It has scaled very well for us at Facebook and Instagram.

## Start With A Mock

Imagine that we already have a JSON API and a mock from our designer. The mock looks like this:

![mock](https://reactjs.org/static/1071fbcc9eed01fddc115b41e193ec11/d4770/thinking-in-react-mock.png)

Our JSON API returns some data that looks like this:

[
  {category: "Sporting Goods", price: "$49.99", stocked: true, name: "Football"},
  {category: "Sporting Goods", price: "$9.99", stocked: true, name: "Baseball"},
  {category: "Sporting Goods", price: "$29.99", stocked: false, name: "Basketball"},
  {category: "Electronics", price: "$99.99", stocked: true, name: "iPod Touch"},
  {category: "Electronics", price: "$399.99", stocked: false, name: "iPhone 5"},
  {category: "Electronics", price: "$199.99", stocked: true, name: "Nexus 7"}
];

## How would you break a mock into a component heirarchy?

The first thing you’ll want to do is to draw boxes around every component (and subcomponent) in the mock and give them all names, and Use the same techniques for deciding if you should create a new function or object. One such technique is the single responsibility principle, that is, a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.

## What is the single responsibility principle and how does it apply to components?

is a computer-programming principle that states that every module, class or function in a computer program should have responsibility over a single part of that program's functionality, and it should encapsulate that part. All of that module, class or function's services should be narrowly aligned with that responsibility.[

## What does it mean to build a ‘static’ version of your application?

To build a static version of your app that renders your data model, you’ll want to build components that reuse other components and pass data using props. props are a way of passing data from parent to child. If you’re familiar with the concept of state, don’t use state at all to build this static version. State is reserved only for interactivity, that is, data that changes over time. Since this is a static version of the app, you don’t need it.

## Once you have a static application, what do you need to add?

To make your UI interactive, you need to be able to trigger changes to your underlying data model. React achieves this with state.

## What are the three questions you can ask to determine if something is state?

1- it passed in from a parent via props? If so, it probably isn’t state.

2- Does it remain unchanged over time? If so, it probably isn’t state.

3- Can you compute it based on any other state or props in your component? If so, it isn’t state.

## How can you identify where state needs to live?

1- Identify every component that renders something based on that state.

2- Find a common owner component (a single component above all the components that need the state in the hierarchy).

3- Either the common owner or another component higher up in the hierarchy should own the state.

4- If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

[Source Site](https://reactjs.org/docs/thinking-in-react.html)



