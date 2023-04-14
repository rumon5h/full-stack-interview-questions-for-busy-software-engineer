# Full Stack Interview Questions For Busy Software Engineer

#### [HTML Interview Questions](HTML.md)
#### [CSS Interview questions](CSS.md)
#### [JavaScript Interview questions](JavaScript.md)
#### [MongoDB Interview questions](MONGODB.md)
#### [Express.js Interview questions](EXPRESS.md)
#### [React.js Interview questions](REACT.md)
#### [Node.js Interview questions](NODE.md)
#### [MERN Stack Interview questions](MERN.md)

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

