# Object-Oriented-Programming-In-Python

Python is a fantastic programming language that allows you to use both functional and 
object-oriented programming paradigms.

All four core aspects of a generic OOP framework are supported by Python's object-oriented
programming system: encapsulation, abstraction, inheritance, and polymorphism.

## What are Classes and Objects?
A class is a collection of instance variables and related methods that define a particular object 
type. You can think of a class as an object's blueprint or template

Attributes are the names given to the variables that make up a class.

A class instance with a defined set of properties is called an object. As a result, the same class 
can be used to construct as many objects as needed.

### How to create a class?
To create a class, we use the keyword class
```
class MyClass:
  y=3
 ```
 we can us MyClass to create objects
 
 ```
val = MyClass()
print(val.y)
```

### The __init__() Function

The examples above are classes and objects in their simplest form, and are not really useful in 
real life applications.

To understand the meaning of classes we have to understand the built-in __init__() function.
All classes have a function called __init__(), which is always executed when the class is being 
initiated.Use the __init__() function to assign values to object properties, or other operations 
that are necessary to do when the object is being created.
```
class Dog:

    def __init__(self, name, age):  
        self.name = name
        self.age = age
g=Dog('German Shephard',3)

print(g.name)
print(g.age)

```

The term self in the attributes refers to the corresponding instances (objects).

```
print(g.name)
print(g.age)
```

## What is Encapsulation?



 
 
