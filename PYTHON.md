# Python Interview Questions

### 1. What is Python?

##### Python is a high-level, interpreted programming language that is easy to learn and supports multiple programming paradigms. It is designed to be concise and readable, and has a vast collection of third-party libraries and modules that make it suitable for a wide range of applications.

### 2. What are the key features of Python?

##### Some of the key features of Python include:

    * Dynamically typed: Variables don't need to be declared before use, and their type can change during runtime.
    * Interpreted: Code is compiled on-the-fly, making development and debugging faster.
    * Object-oriented: Encourages the use of object-oriented programming principles.
    * Extensible: Python has a large number of third-party libraries and modules that can be easily integrated into your code.
    * Easy to learn: Python has a clean syntax and is easy to read, making it a great language for beginners.
    * Cross-platform: Python code can run on various operating systems, including Windows, Linux, and macOS.

###3. What are some of the data types in Python?

##### Some of the data types in Python include:

    * Integers: whole numbers, e.g. 1, 2, 3, etc.
    * Floats: decimal numbers, e.g. 1.5, 2.75, etc.
    * Strings: sequences of characters, e.g. "hello", "world", etc.
    * Booleans: logical values that are either True or False.
    * Lists: ordered sequences of elements, e.g. [1, 2, 3], ["hello", "world"], etc.
    * Tuples: ordered, immutable sequences of elements, e.g. (1, 2, 3), ("hello", "world"), etc.
    * Dictionaries: unordered collections of key-value pairs, e.g. {"name": "John", "age": 30}, etc.

### 4. What is the difference between a list and a tuple?

##### The main difference between a list and a tuple is that a list is mutable (i.e. can be modified after creation), whereas a tuple is immutable (i.e. cannot be modified after creation). Lists are created using square brackets, e.g. [1, 2, 3], while tuples are created using parentheses, e.g. (1, 2, 3). Another difference is that lists are usually used to store homogeneous items (i.e. items of the same type), while tuples can store heterogeneous items (i.e. items of different types).

### 5. What is a lambda function in Python?

##### A lambda function is a small, anonymous function in Python that can have any number of arguments, but can only have one expression. Lambda functions are typically used for one-time operations where defining a separate function would be overkill. Lambda functions are defined using the lambda keyword, e.g. lambda x, y: x + y.

### 6. How do you handle errors and exceptions in Python?

##### In Python, errors and exceptions are handled using the try...except block. The try block contains the code that may raise an exception, while the except block contains the code that will handle the exception. For example:

```python

try:
    # some code that may raise an exception
except SomeException:
    # code to handle the exception
```
### 7. What is the difference between `__str__` and `__repr__` in Python?

##### Both `__str__` and `__repr__` are methods in Python that are used to represent an object as a string, but they serve different purposes.

##### The `__repr__` method returns a string that represents a printable version of an object, which can be used to recreate the object. It is typically used for debugging and development purposes. If the `__repr__` method is not defined for a class, the default implementation will return a string that includes the class name and the memory address of the object.

##### On the other hand, the `__str__` method returns a string that represents a human-readable version of an object. It is typically used to display the object to the end-user. If the `__str__` method is not defined for a class, Python will look for the `__repr__` method and use that instead.

```python
Here is an example that demonstrates the difference between the two methods:

class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def __repr__(self):
        return f'Person(name={self.name}, age={self.age})'

    def __str__(self):
        return f'{self.name} ({self.age})'

p = Person('John', 30)

# calls __repr__ implicitly
print(repr(p))   # Output: Person(name=John, age=30)

# calls __str__ implicitly
print(p)         # Output: John (30)

```
##### In this example, the __repr__ method returns a string that includes the name and age of the person, while the __str__ method returns a more human-readable string that only includes the name and age. When the repr or str function is called on the Person object, the corresponding method is invoked.
