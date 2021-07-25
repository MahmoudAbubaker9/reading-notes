# State and Props

## component lifecycle events
React lets you define components as classes or functions. The methods that you are able to use on these are called lifecycle events. These methods can be called during the lifecycle of a component, and they allow you to update the UI and application states.

## the three phases of the component lifecycle:

1- Mounting:
When an instance of a component is being created and inserted into the DOM it occurs during the mounting phase. Constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount all occur in this order during mounting.

2- Updating:
Anytime a component is updated or state changes then it is rerendered. These lifecycle events happen during updating in this order. static getDerivedStateFromProps, shouldComponentUpdate, render, getSnapshotBeforeUpdate, componentDidUpdate, UNSAFE_componentWillUpdate, UNSAFE_componentWillReceiveProps

3- Unmounting:
The final phase of the lifecycle if called when a component is being removed from the DOM. componentWillUnmount is the only lifecycle event during this phase.

constructor()
The constructor for a React component is called before it is mounted.If the component is a subclass you should call super(props), or the props will be undefined. constructors can be used to assign state using this.state or to bind event handle methods to an instance.

Avoid using this.setState() in the constructor because it can lead to side effects, and it is unnecessary.

static getDerivedStateFromProps()
This method exists for rare cases where the state relies on changes in props over time.

render()
Render is the only required method in a class component. It will examine this.props and this.state when called. The render function should not modify the component state because it would cause a lot of bugs by changing the state every time it rerenders.

componentDidMount()
This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions.

shouldComponentUpdate()
The default behavior in react is to rerender after every state change. Setting shouldComponentUpdate() to false allows you to prevent this from happening. This is in order to optimize performance. If you want to use this method, it may be better to use PureComponent instead, which performs a shallow comparison of props and state. I

getSnapshotBeforeUpdate()
This is another rarely used method that allows you to capture a picture of the DOM to check it before actually changing anything on the DOM.

componentDidUpdate()
This method is useful for performing network requests after a change has occurred.

componentWillUnmount()
This method allows you to clean up the DOM and netwrok requests/ subscriptions.

## React State Vs Props

What types of things can you pass in the props?
Any type of data can be passed throught the props.

What is the big difference between props and state?
Props passes data into the component (child can't alter parent  data)
state is handeled inside of the component (child can alter parent  data)

When do we rerender our application?
When we change the state of that component the comopnent gets rerendered.

What are some examples of things that we could store in state?
input elment check-box select-box





