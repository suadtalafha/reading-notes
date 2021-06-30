# Putting it all together

### 1-How would you break a mock into a component heirarchy?
 We will want to do is to draw boxes around every component and subcomponent in the mock and give them all names. And about how to decide which one is the component and which ones are the sub,it’s that the component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.

### 2-What is the single responsibility principle and how does it apply to components?

a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.All of that module, class or function’s services should be narrowly aligned with that responsibility.

### 3-What does it mean to build a ‘static’ version of your application?

To build a static version of your app that renders your data model, you’ll want to build components that reuse other components and pass data using props props are a way of passing data from parent to child, and will not be using the state at all while building the static application.

### 4-Once you have a static application, what do you need to add?

props are a way of passing data from parent to child. If you’re familiar with the concept of state, don’t use state at all to build this static version. State is reserved only for interactivity, that is, data that changes over time. Since this is a static version of the app, you don’t need it.

### 5-What are the three questions you can ask to determine if something is state?

1- Is it passed in from a parent via props? If so, it probably isn’t state.

2- Does it remain unchanged over time? If so, it probably isn’t state.

3- Can you compute it based on any other state or props in your component? If so, it isn’t state.

### 6-How can you identify where state needs to live?

- Identify every component that renders something based on that state.

- Find a common owner component (a single component above all the components that need the state in the hierarchy).

- Either the common owner or another component higher up in the hierarchy should own the state.

- If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

![image](https://masteringbusinessanalysis.com/wp-content/uploads/2015/09/Putting-it-all-togther-1080x675.jpg)