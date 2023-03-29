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
