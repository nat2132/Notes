# Class 6 Mapping in Python

Mapping in Python is an important concept that enables you to derive a new list from an existing one, with modifications to each element. This is typically done using the built-in `map()` function, which takes two or more arguments: a function and one or more iterables, represented in the format `map(function, iterable, ...)`.

The function you provide is applied to every item in the input iterable. Interestingly, the `map()` function returns a map object which is a lazy iterable. This means that it doesn't store all the results at once but generates them as needed, which can be a significant memory-saver for large inputs.

Here's a simple example to illustrate this:

```python
# Function to double the value
def double(n):
    return n * 2

numbers = [1, 2, 3, 4]
result = map(double, numbers)
print(list(result))  # Output: [2, 4, 6, 8]

```

In the example above, the `double` function is applied to every item in the `numbers` list. The result is a new list where each number is the double of the corresponding number in the original list.

Additionally, you can use `map()` with multiple iterables. The function should have as many arguments as the number of iterables. The iterables should be of the same length. If not, the function stops when the smallest iterable is exhausted. Here's an example:

```python
# Function to add two values
def add(a, b):
    return a + b

numbers1 = [1, 2, 3]
numbers2 = [4, 5, 6]
result = map(add, numbers1, numbers2)
print(list(result))  # Output: [5, 7, 9]

```

In this case, the `add` function is applied to each pair of elements from `numbers1` and `numbers2`, resulting in a new list with each number being the sum of the corresponding numbers in the original lists.

# Object Oriented Programming in Python

Object-Oriented Programming (OOP) in Python is a programming paradigm that is built around the concept of objects. An object is an entity that holds data along with the functions (methods) that can operate on that data. Objects are instances of classes, which can be thought of as blueprints for creating objects.

Python is inherently an object-oriented language and has been since its inception. Almost everything in Python is an object, with its properties and methods.

Here's a simple example to illustrate the concept of classes and objects:

```python
# Define a class
class Car:
    def __init__(self, color, brand):
        self.color = color
        self.brand = brand

    def display_info(self):
        print("This car is a", self.color, self.brand)

# Create an object of the Car class
my_car = Car("red", "Toyota")
my_car.display_info()  # Output: This car is a red Toyota

```

In the example above, `Car` is a class that has two attributes: `color` and `brand`. It also has a method `display_info` that prints the color and brand of the car. `my_car` is an object of the `Car` class, with color as 'red' and brand as 'Toyota'. When we call the method `display_info` on `my_car`, it prints 'This car is a red Toyota'.

In addition to the basic OOP concepts, Python also supports inheritance, which allows one class (child class) to inherit the attributes and methods of another class (parent class). It also supports encapsulation, which restricts access to some of the object's components, and polymorphism, which allows one interface to be used for a general class of actions.

Python supports several characteristics of Object-Oriented Programming, including:

- **Classes and Objects**: Python allows the definition of classes and creation of objects from those classes. Each object can have properties and behaviors, defined by its class.
- **Encapsulation**: Python provides methods to define private, protected and public attributes and methods which can provide a way to restrict access to certain methods and variables in the object.
- **Inheritance**: Python allows a class to inherit attributes and methods from another class, enabling code reuse and complexity management.
- **Polymorphism**: In Python, one function or an operator may behave differently in different contexts, which is known as polymorphism.
- **Abstraction**: Python allows for creating complex real-world models by ignoring unnecessary details and displaying only the needed ones.
- **Composition**: Python enables a class to contain an object of another class.
- **Dynamic Typing**: Python is dynamically typed. This means that the type of a value is checked only at runtime, and the language automatically keeps track of the type of an object.