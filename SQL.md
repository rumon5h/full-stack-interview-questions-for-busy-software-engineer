# SQL Interview Questions

### 1. What is SQL?

##### SQL stands for Structured Query Language, which is a programming language used to manage and manipulate relational databases. It is used to perform various operations such as creating, modifying, and deleting tables, retrieving data from tables, and inserting new data into tables.

### 2. What are the different types of SQL commands?

##### SQL commands can be classified into four types:

    * DDL (Data Definition Language) commands: These commands are used to create, alter, and delete database objects such as tables, indexes, and views.

    * DML (Data Manipulation Language) commands: These commands are used to manipulate data stored in the database, such as inserting, updating, and deleting records.

    * DCL (Data Control Language) commands: These commands are used to control the access to the database, such as granting and revoking privileges to users.

    * TCL (Transaction Control Language) commands: These commands are used to manage transactions in the database, such as committing or rolling back transactions.

### 3. What is a primary key?

##### A primary key is a column or a set of columns in a table that uniquely identifies each row in the table. It is used to enforce data integrity and to create relationships between tables. A primary key column cannot contain null values.

```sql

CREATE TABLE Customers (
  customer_id INT PRIMARY KEY,
  first_name VARCHAR(50),
  last_name VARCHAR(50),
  email VARCHAR(100)
);
```

### 4. What is a foreign key?

##### A foreign key is a column or a set of columns in a table that refers to the primary key of another table. It is used to create relationships between tables and to enforce referential integrity. A foreign key column can contain null values if the relationship is optional.

``` sql

CREATE TABLE Orders (
  order_id INT PRIMARY KEY,
  customer_id INT,
  order_date DATE,
  FOREIGN KEY (customer_id) REFERENCES Customers(customer_id)
);
```

### 5. What is a join?

##### A join is an operation used to combine data from two or more tables based on a related column between them. There are several types of joins in SQL, such as inner join, left join, right join, and full outer join.

```sql

SELECT *
FROM Orders
INNER JOIN Customers
ON Orders.customer_id = Customers.customer_id;
```

### 6. What is normalization?

##### Normalization is the process of organizing data in a database to reduce redundancy and dependency. It involves dividing large tables into smaller tables and defining relationships between them to minimize data duplication and ensure data integrity.

### 7. What is a subquery?

##### A subquery is a query that is nested inside another query. It is used to retrieve data from one or more tables and then use that result set as a condition or a value in another query.

```sql

SELECT *
FROM Customers
WHERE customer_id IN (
  SELECT customer_id
  FROM Orders
  WHERE order_date > '2022-01-01'
);
```

### 8. What is a view?

##### A view is a virtual table that is derived from one or more tables or views. It is used to simplify complex queries and to provide a simplified interface to the underlying data.

```sql

CREATE VIEW CustomerOrders AS
SELECT Customers.customer_id, Orders.order_id, Orders.order_date
FROM Customers
INNER JOIN Orders
ON Customers.customer_id = Orders.customer_id;
```

### 9. What is a stored procedure?

##### A stored procedure is a pre-compiled set of SQL statements that are stored in the database and can be executed by calling the procedure. It is used to encapsulate complex logic and business rules that can be reused by multiple applications and scripts.

##### Stored procedures are commonly used for tasks such as data validation, data transformation, and complex data retrieval. They can also be used to improve performance by reducing network traffic and improving query execution time.

##### Here is an example of a stored procedure that retrieves all customers who have placed an order within a specific date range:

```sql

CREATE PROCEDURE GetCustomersWithOrders
    @StartDate DATE,
    @EndDate DATE
AS
BEGIN
    SELECT DISTINCT Customers.*
    FROM Customers
    INNER JOIN Orders
    ON Customers.customer_id = Orders.customer_id
    WHERE Orders.order_date BETWEEN @StartDate AND @EndDate
END

To execute the stored procedure, you can call it by its name and pass in the required parameters:
```
```sql

EXEC GetCustomersWithOrders '2022-01-01', '2022-12-31'
```
##### This will return a result set containing all customers who have placed an order between January 1st, 2022 and December 31st, 2022.
