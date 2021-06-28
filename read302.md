# Component Lifecycle Events
React lets you define components as classes or functions. The methods that you are able to use on these are called lifecycle events.

![image](https://miro.medium.com/max/5560/1*CtXr4JMSIGGdxsl5dA58jw.png)

## The three phases of the component lifecycle

1-Mounting When an instance of a component is being created and inserted into the DOM it occurs during the mounting phase. Constructor, static getDerivedStateFromProps, render, componentDidMount, and U2-NSAFE_componentWillMount all occur in this order during mounting.
3-Updating Anytime a component is updated or state changes then it is rerendered.
4-Unmounting The final phase of the lifecycle if called when a component is being removed from the DOM. componentWillUnmount is the only lifecycle event during this phase.


## Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?
componentDidMount
## What is the very first thing to happen in the lifecycle of React?
Mounting :
When an instance of a component is being created and inserted into the DOM it occurs during the mounting phase. Constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount all occur in this order during mounting.


1. What types of things can you pass in the props?
The values can be any data type, from strings to functions, objects, etc
initial values
values we did not change them.
2. What is the big difference between props and state?
props you bass into a component and state is handled and update inside of that component and props are handled and update outside of the component

3. When do we re-render our application?
when we change the state inside app

4.What are some examples of things that we could store in state?
Inside of a form


## State and Lifecycle
Steps to Converting a Function to a Class You can convert a function component like Clock to a class in five steps:

Create an ES6 class, with the same name, that extends React.Component.
Add a single empty method to it called render().
Move the body of the function into the render() method.
Replace props with this.props in the render() body.
Delete the remaining empty function declaration.
Using State :

## Do Not Modify State Directly
State Updates May Be Asynchronous
State Updates are Merged


### Handling Events
Handling events with React elements is very similar to handling events on DOM elements. There are some syntax differences:

React events are named using camelCase, rather than lowercase.
With JSX you pass a function as the event handler, rather than a string.