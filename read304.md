# React and Forms
1-What is a ‘Controlled Component’?

it’s convenient to have a JavaScript function that handles the submission of the form and has access to the data that the user entered into the form ,The form elements in HTML they maintain their own state and update it based on user input, but in React,the state for them is typically kept in the state property of components, and only updated with setState().So Controlled Component allow us to combine the two by making the React state be the single source of truth ,which means that the React component that renders a form also controls what happens in that form on subsequent user input.

2-Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

We update it as soon as they enter , because we are using an event handler that is runs on every keystroke to update the React state, the displayed value will update as the user types.

3-How do we target what the user is entering if we have an event handler on an input field?

{this.handleChange} 

## The Conditional (Ternary) Operator Explained
1-Why would we use a ternary operator?

its shorter thin the if statement , redues time and more cleanr thin if statement

2-Rewrite the following statement using a ternary statement:

if(x===y){ console.log(true); } else { console.log(false); }

>the ans =====> x===y ? (console.log(true)) : (console.log(false))


![image](https://pbs.twimg.com/media/EKzwxZ4WkAAwjlw.jpg)