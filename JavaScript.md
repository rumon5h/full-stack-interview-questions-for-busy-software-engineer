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
