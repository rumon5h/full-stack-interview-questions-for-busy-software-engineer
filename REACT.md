# React Interview Questions

### What is React.js and why is it used?

##### React.js is an open-source JavaScript library used for building user interfaces or UI components. It is used because it allows developers to create reusable UI components and update the UI components in real-time without having to reload the entire web page.

```javascript
Code Example:

A simple React component that renders a button:

import React from 'react';

function Button(props) {
  return <button onClick={props.onClick}>{props.text}</button>;
}
```
### What is JSX in React?

##### JSX stands for JavaScript XML, which is an extension to the JavaScript language syntax that allows developers to write HTML-like code in their JavaScript files. JSX makes it easier to create and manipulate UI elements in React.

```javascript
Code Example:

A simple example of JSX syntax:

import React from 'react';

function Hello() {
  return (
    <div>
      <h1>Hello, world!</h1>
      <p>Welcome to my React app.</p>
    </div>
  );
}
```
### What is the virtual DOM in React?

##### The virtual DOM is a JavaScript representation of the actual DOM (Document Object Model) that React uses to optimize rendering performance. When a change is made to the virtual DOM, React compares the new virtual DOM with the old virtual DOM and only updates the parts that have changed, which makes the process faster and more efficient.

```javascript
Code Example:

A simple example of updating the virtual DOM in React:

import React, { useState } from 'react';

function Counter() {
  const [count, setCount] = useState(0);

  function handleClick() {
    setCount(count + 1);
  }

  return (
    <div>
      <p>You clicked {count} times.</p>
      <button onClick={handleClick}>Click me!</button>
    </div>
  );
}
```
### What is the difference between a class component and a functional component in React?

##### A class component is a React component that extends the React.Component class and defines a render method that returns a React element. A functional component is a React component that is defined as a function that returns a React element.

```javascript
Code Example:

A simple class component and functional component in React:

import React from 'react';

// Class Component
class Greeting extends React.Component {
  render() {
    return <h1>Hello, {this.props.name}!</h1>;
  }
}

// Functional Component
function Greeting(props) {
  return <h1>Hello, {props.name}!</h1>;
}
```

### What is Redux in React and why is it used?

##### Redux is a state management library for React that allows developers to manage application state in a predictable way. It is used to store the global state of an application and makes it easier to share state between different components.
