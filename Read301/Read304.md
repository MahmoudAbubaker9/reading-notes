# React and Forms


## React Docs - Forms

### Forms

HTML form elements work a bit differently from other DOM elements in React, because form elements naturally keep some internal state

1- What is a ‘Controlled Component’?

In HTML, form elements such as input, textarea, and select typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with setState().

We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a “controlled component”.

2- Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

It is updated immediately after entering the variable.

>because when usingthe controlled component, the component state is the single source of truth.


Since the value attribute is set on our form element, the displayed value will always be this.state.value, making the React state the source of truth. Since handleChange runs on every keystroke to update the React state, the displayed value will update as the user types.


3- How do we target what the user is entering if we have an event handler on an input field?

When you need to handle multiple controlled input elements, you can add a name attribute to each element and let the handler function choose what to do based on the value of event.target.name.


## Controlled Components 

1- The file input Tag : Because its value is read-only, it is an uncontrolled component in React. It is discussed together with other uncontrolled components

2- The select Tag : Note that the Coconut option is initially selected, because of the selected attribute. React, instead of using this selected attribute, uses a value attribute on the root select tag. This is more convenient in a controlled component because you only need to update it in one place. 

3- The textarea Tag 

# The Conditional (Ternary) Operator Explained

1- Why would we use a ternary operator?

Programmers use the ternary operator for decision making in place of longer if and else conditional statements


2- Rewrite the following statement using a ternary statement

let text = (x===y ? console.log(true) : console.log(false))