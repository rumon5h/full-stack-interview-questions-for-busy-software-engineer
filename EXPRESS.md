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
