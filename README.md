# Full Stack Interview Questions For Busy Software Engineer

#### [MERN Stack Interview questions](MERN.md)
#### [HTML Interview Questions](HTML.md)
#### [CSS Interview questions](CSS.md)
#### [JavaScript Interview questions](JavaScript.md)
#### [TypeScript Interview questions](TYPESCRIPT.md)
#### [MongoDB Interview questions](MONGODB.md)
#### [Express.js Interview questions](EXPRESS.md)
#### [React.js Interview questions](REACT.md)
#### [Node.js Interview questions](NODE.md)
#### [Next.js Interview questions](NEXT.md)
#### [SQL Interview questions](SQL.md)
#### [Python Interview questions](PYTHON.md)
#### [DJANGO Interview questions](DJANGO.md)


## HTML Interview Questions

### Q1. What is HTML?

##### HTML stands for HyperText Markup Language. It is a standard markup language used for creating web pages and web applications.

### Q2. What are the basic elements of HTML?

##### The basic elements of HTML are:

    * <html>: Defines the start and end of an HTML document.
    * <head>: Contains meta information about the document such as title, keywords, etc.
    * <body>: Contains the content of the document that is visible to the user.
    * <title>: Defines the title of the document that appears in the browser's title bar.

### Q3. What is the difference between HTML and XHTML?

##### HTML and XHTML are both markup languages used for creating web pages. The main difference between the two is that HTML is an SGML-based language, whereas XHTML is an XML-based language. This means that XHTML is stricter and requires all elements to be properly closed, while HTML allows for some flexibility in this regard.

### Q4. What is the difference between <div> and <span>?

##### Both <div> and <span> are used as containers for other HTML elements. The main difference between the two is that <div> is a block-level element, while <span> is an inline element. This means that <div> creates a new line and takes up the full width of its parent element, while <span> does not create a new line and only takes up as much space as its contents require.

  
### Q5. What is the purpose of the alt attribute in an `<img>` tag?

##### The alt attribute in an `<img>` tag is used to provide alternative text for the image in case it cannot be displayed. This can be due to a slow internet connection, a broken image link, or for accessibility purposes for users with visual impairments. The alt text should describe the content of the image in a concise and meaningful way.

### Q6. What is the difference between a class and an ID in HTML?

##### Both classes and IDs are used to identify specific HTML elements. The main difference between the two is that a class can be used to apply styles to multiple elements, while an ID should only be used to identify a single unique element. Additionally, an ID must be unique within the document, while a class can be used multiple times.

### Q7. What is the purpose of the `<form>` element in HTML?

##### The `<form>` element is used to create a form on a web page that allows users to input data. It can contain various types of input elements such as text boxes, checkboxes, radio buttons, and submit buttons. The data entered by the user can be sent to a server-side script for processing using the action attribute.

### Q8. What is the purpose of the `<meta>` element in HTML?

##### The `<meta>` element is used to provide metadata about the HTML document. This includes information such as the document's author, keywords, description, and character encoding. This metadata is used by search engines to better index the page, and by browsers to display the page correctly.
  
### Q9. What is the purpose of the `<link>` element in HTML?

##### The `<link>` element is used to link to external resources such as stylesheets, scripts, and other web pages. It can be used to define the relationship between the current document and the linked resource using the rel attribute.
  
### Q10. What is the purpose of the target attribute in an `<a>` tag?

### The target attribute in an `<a>` tag is used to specify where the linked document should be displayed when clicked. It can be

  
# CSS Interview Questions

### 1. What is CSS?
    
##### Answer: CSS stands for Cascading Style Sheets. It is a style sheet language that is used to describe the look and formatting of a document written in HTML.

### What are the advantages of using CSS?

##### Answer: CSS allows for a separation of presentation and content, making it easier to maintain and update styles across a website. It also allows for greater control over the layout and design of a website, making it more user-friendly and accessible.

### 2. What is the syntax of a CSS rule?
    
##### Answer: A CSS rule consists of a selector and a declaration block. The selector identifies the HTML element that the rule applies to, and the declaration block contains one or more declarations, which specify the style properties and values for the selected element.

### What are selectors in CSS?

##### Answer: Selectors are used to target specific HTML elements in order to apply styling rules. They can be based on element type, class, ID, attribute, or any combination of these.

### What is the box model in CSS?

##### Answer: The box model is a way of representing an HTML element as a rectangular box with content, padding, borders, and margins. The width and height of the box are determined by the content, and the padding, borders, and margins are added to the outside of the content box.

### What is the difference between margin and padding in CSS?

##### Answer: Margin refers to the space between an element and its neighboring elements, while padding refers to the space between an element's content and its borders.

### What is the difference between inline and block elements in CSS?

##### Answer: Inline elements flow within the text of a document and do not create line breaks, while block elements create a new line and take up the full width of their parent container.

### What is the "float" property in CSS?

##### Answer: The float property is used to specify whether an element should be floated to the left or right of its container. It is commonly used for creating multi-column layouts.

### What is a CSS framework?

##### Answer: A CSS framework is a pre-written set of CSS styles and rules that can be used to quickly and easily build websites or web applications. It typically includes a grid system, pre-built UI components, and other useful features.

### What are media queries in CSS?

##### Answer: Media queries are used to apply different styles to a document based on the device or screen size that it is being viewed on. They allow for responsive design, which can adapt to different screen sizes and resolutions.

# JavaScript Interview Questions and Answers

### 1. What is JavaScript?

##### JavaScript is a high-level programming language that is often used in web development to create interactive and dynamic websites. It is an object-oriented language that supports a wide range of features such as functions, arrays, objects, and loops.

### 2. What is the difference between == and === operators in JavaScript?

##### The '==' operator compares two values for equality, but it does not take into account their data types. On the other hand, the '===' operator compares two values for equality and also checks their data types.

```javascript
console.log(1 == '1');  // true
console.log(1 === '1');  // false
```

### 3. What are closures in JavaScript?

##### Closures are functions that have access to the variables defined in their outer function, even after the outer function has returned. Closures are often used to create private variables in JavaScript.

```javascript

function outerFunction() {
  var outerVariable = 'I am outer';

  function innerFunction() {
    console.log(outerVariable);
  }

  return innerFunction;
}

var innerFunctionRef = outerFunction();
innerFunctionRef();  // Output: I am outer
```

### 4. What is the difference between null and undefined in JavaScript?

##### In JavaScript, 'null' is a value that represents the intentional absence of any object value, whereas 'undefined' is a value that represents the absence of any value.

```javascript
var variable1;  // undefined
var variable2 = null;  // null
```
### 5. What is the 'this' keyword in JavaScript?

##### The 'this' keyword in JavaScript refers to the object that is currently executing the code. The value of 'this' can change depending on how a function is called.

```javascript
var person = {
  firstName: 'Md. Rumon',
  lastName: 'Khan',
  fullName: function() {
    console.log(this.firstName + ' ' + this.lastName);
  }
};

person.fullName();  // Output: Md. Rumon Khan
```
### 6. What is a callback function in JavaScript?

##### A callback function is a function that is passed as an argument to another function and is called when the parent function has finished executing. Callback functions are often used to handle asynchronous operations in JavaScript.

```javascript
function fetchData(callback) {
  // Simulate an asynchronous operation
  setTimeout(function() {
    var data = { name: 'Rumon', age: 21 };
    callback(data);
  }, 1000);
}

fetchData(function(data) {
  console.log(data);  // Output: { name: 'Rumon', age: 21 }
});
```
### 7. What is the difference between let and var in JavaScript?

##### The 'let' keyword was introduced in ES6 and is used to declare variables with block scope. On the other hand, the 'var' keyword is used to declare variables with function scope.

```javascript 
if (true) {
  var variable1 = 'I am var';
  let variable2 = 'I am let';
}

console.log(variable1);  // Output: I am var
console.log(variable2);  // Throws ReferenceError: variable2 is not defined
```
### 8. What is the use of the 'use strict' directive in JavaScript?

##### The 'use strict' directive is used to enforce stricter parsing and error handling in JavaScript. When used, it enables a stricter mode of execution and disallows certain actions that are allowed in non-strict mode.

```javascript
'use strict';

x = 3.14;  // Throws ReferenceError
```

# MongoDB Interview Questions

### Question 1: What is MongoDB?

##### Answer: MongoDB is a popular open-source NoSQL document-oriented database program. It stores data in flexible, JSON-like documents, meaning fields can vary from document to document and data structure can be changed over time.

### Question 2: What are the advantages of using MongoDB?

##### Answer:

    * High Performance and Scalability
    * Dynamic Schema
    * High Availability and Automatic Sharding
    * Rich Query Language
    * Indexing Support
    * Document-Oriented Storage
    * Flexible Data Model

### Question 3: What is a replica set in MongoDB?

##### Answer: A replica set is a group of MongoDB servers that maintain the same data set. It provides redundancy and high availability, allowing for automatic failover and recovery in case of server failure. In a replica set, one server is designated as the primary node, and the others are secondary nodes.

### Question 4: What is sharding in MongoDB?

##### Answer: Sharding is a technique used to horizontally scale MongoDB databases across multiple servers. It divides a large collection into smaller, more manageable chunks called shards, which are distributed across multiple servers. This helps to improve performance, scalability and availability of the database.

### Question 5: How do you connect to MongoDB using Node.js?

##### Answer: To connect to MongoDB using Node.js, you need to use a MongoDB driver. Here's an example of how to connect to a MongoDB server using the mongodb driver in Node.js:

``` javascript

const MongoClient = require('mongodb').MongoClient;
const uri = 'mongodb://localhost:27017/mydb';

MongoClient.connect(uri, function(err, client) {
  if (err) throw err;
  const db = client.db('mydb');
  console.log('Connected to MongoDB!');
  client.close();
});

In this example, we're connecting to a MongoDB server running on localhost on port 27017 and opening a database called mydb. We then log a message to the console and close the connection.

```
### Question 6: How do you create a collection in MongoDB?

##### Answer: To create a collection in MongoDB, you can use the createCollection method. Here's an example:

``` javascript

const MongoClient = require('mongodb').MongoClient;
const uri = 'mongodb://localhost:27017/mydb';

MongoClient.connect(uri, function(err, client) {
  if (err) throw err;
  const db = client.db('mydb');
  db.createCollection('customers', function(err, res) {
    if (err) throw err;
    console.log('Collection created!');
    client.close();
  });
});

In this example, we're creating a collection called customers in the mydb database. If the collection already exists, the createCollection method will not create a new collection.
```

### Question 7: How do you insert documents into a collection in MongoDB?

##### Answer: To insert documents into a collection in MongoDB, you can use the `insertOne` or `insertMany` method.

# Express Interview Questions

### Question 1: What is Express.js?

##### Answer: Express.js is a popular web application framework for Node.js that provides a set of robust features for building web and mobile applications. It is built on top of Node.js and offers a simple, yet powerful set of tools for building HTTP servers, handling routes, middleware, and much more.

### Question 2: What is middleware in Express.js?

##### Answer: Middleware in Express.js is a series of functions that are executed sequentially during the request-response cycle of an HTTP request. Each middleware function can modify the request and response objects, and can pass control to the next middleware function in the chain.

### Question 3: How to handle routing in Express.js?

##### Answer: Routing in Express.js is handled using the express.Router() method. This method returns an instance of a router, which can be used to define routes for the application. Here's an example of how to define a simple route using the router:

```javascript

const express = require('express')
const router = express.Router()

router.get('/', (req, res) => {
  res.send('Hello, World!')
})

module.exports = router
```

### Question 4: How to handle errors in Express.js?

##### Answer: Errors in Express.js can be handled using middleware functions that have four arguments instead of the usual three. The additional argument is an error object that contains information about the error that occurred. Here's an example of an error handling middleware:

```javascript

app.use((err, req, res, next) => {
  console.error(err.stack)
  res.status(500).send('Something broke!')
})
```

### Question 5: How to use templates in Express.js?

##### Answer: Templates in Express.js can be used to generate HTML dynamically on the server-side. Popular templating engines for Express.js include EJS, Handlebars, and Pug. Here's an example of how to use EJS in Express.js:

```javascript

const express = require('express')
const app = express()

app.set('view engine', 'ejs')

app.get('/', (req, res) => {
  res.render('index', { name: 'John' })
})

app.listen(3000, () => {
  console.log('Server listening on port 3000')
})

This code sets the view engine to EJS, defines a route that renders an EJS template called index, and passes an object with the property name set to 'John' to the template.

```

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

# Node Interview Questions

### Q1: What is Node.js?

##### A: Node.js is an open-source, cross-platform JavaScript runtime environment that allows developers to run JavaScript on the server-side. It is built on top of the V8 JavaScript engine from Google Chrome and provides an event-driven, non-blocking I/O model that makes it lightweight and efficient.

### Q2: What is the difference between Node.js and other server-side frameworks like Ruby on Rails and Django?

##### A: Node.js differs from traditional server-side frameworks like Ruby on Rails and Django in several ways:

    * Node.js is built on top of the V8 JavaScript engine, while Ruby on Rails is built on top of the Ruby language and Django is built on top of Python. This means that Node.js is much faster and more efficient than these frameworks.
    * Node.js is event-driven and non-blocking, while Ruby on Rails and Django are blocking frameworks. This means that Node.js can handle large amounts of I/O operations without slowing down or blocking the server.
    * Node.js is designed to handle real-time, data-intensive applications like chat apps and streaming services, while Ruby on Rails and Django are better suited for building traditional web applications.

### Q3: What is callback hell in Node.js and how can it be avoided?

##### A: Callback hell is a common issue in Node.js where nested callbacks can become difficult to read and maintain. It can be avoided by using promises, async/await, or a library like Async.js.

```javascript
Here's an example of using promises to avoid callback hell:

function getUsers() {
  return new Promise((resolve, reject) => {
    db.query('SELECT * FROM users', (err, result) => {
      if (err) {
        reject(err);
      } else {
        resolve(result);
      }
    });
  });
}

function getUserById(id) {
  return new Promise((resolve, reject) => {
    db.query('SELECT * FROM users WHERE id = ?', [id], (err, result) => {
      if (err) {
        reject(err);
      } else {
        resolve(result);
      }
    });
  });
}

getUsers()
  .then((users) => {
    return getUserById(users[0].id);
  })
  .then((user) => {
    console.log(user);
  })
  .catch((err) => {
    console.error(err);
  });
```
### Q4: What is middleware in Node.js and how is it used?

##### A: Middleware in Node.js is a function that receives the request and response objects, and the next middleware function in the application's request-response cycle. It can be used to modify the request or response objects, or to perform other tasks like logging, authentication, and error handling.

```javascript
Here's an example of a middleware function that logs the request method and URL:

function logMiddleware(req, res, next) {
  console.log(`[${req.method}] ${req.url}`);
  next();
}

app.use(logMiddleware);
```
### Q5: How can you handle errors in Node.js?

##### A: Errors in Node.js can be handled using try-catch blocks, or by using the error handling middleware function in Express.

```javascript
Here's an example of using try-catch blocks to handle errors:

try {
  const result = someFunction();
  console.log(result);
} catch (err) {
  console.error(err);
}
```

  # MEEN Stack Interview Questions
  
   ### What is MERN stack?
    
   ##### MERN stack is a popular web development stack that consists of four main components: MongoDB, Express.js, React.js, and Node.js. MongoDB is used as the database, Express.js is used as the web application framework, React.js is used for the user interface, and Node.js is used as the server-side runtime environment.

   ### What is the difference between React and Angular?

   ##### React is a JavaScript library for building user interfaces, while Angular is a full-fledged framework for building complex web applications. React relies on a component-based architecture, whereas Angular relies on a modular architecture.

   ### What is JSX in React?

   ##### JSX stands for JavaScript XML, and it is a syntax extension for JavaScript that allows you to write HTML-like code in your JavaScript files. JSX is used in React to define the structure of the user interface.

   ### What is a virtual DOM in React?

   ##### The virtual DOM is a lightweight representation of the actual DOM in memory. It is used by React to optimize the performance of updates to the user interface. When a change is made to the virtual DOM, React compares it to the previous version of the virtual DOM and only updates the parts that have changed, rather than re-rendering the entire user interface.

   ### What is Express.js?

   ##### Express.js is a popular web application framework for Node.js. It provides a simple and flexible way to handle HTTP requests and responses, as well as middleware for handling common tasks such as authentication and error handling.

   ### What is middleware in Express.js?

   ##### Middleware is a function that sits between the client and the server in an Express.js application. It can perform tasks such as authentication, logging, and error handling, and it can modify the request and response objects before they are sent back to the client.

   ### What is Node.js?

   ##### Node.js is a server-side runtime environment for JavaScript. It allows you to run JavaScript on the server, which enables you to build scalable and high-performance web applications.

   ### What is MongoDB?

   ##### MongoDB is a popular NoSQL database that uses a document-oriented data model. It stores data in flexible JSON-like documents, which makes it easy to work with data that has a complex and dynamic structure.

   ### What is the difference between SQL and NoSQL databases?

   ##### SQL databases use a structured data model, which means that data is stored in tables with predefined columns and rows. NoSQL databases use a document-oriented data model, which means that data is stored in flexible JSON-like documents.

   ### What is RESTful API?

   ##### A RESTful API is an architectural style for building web APIs. It uses HTTP methods such as GET, POST, PUT, and DELETE to perform CRUD (create, read, update, delete) operations on resources, and it uses URLs to identify the resources. A RESTful API is stateless, which means that each request contains all the information necessary to complete the request.
```

   I hope these answers help you prepare for your MERN stack web developer interview! Good luck!

```