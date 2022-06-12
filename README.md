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
mg=Dog('German Shephard',3)

print(mg.name)
print(mg.age)

```

The term self in the attributes refers to the corresponding instances (objects).

```
print(mg.name)
print(mg.age)
```

## What is Encapsulation?

Encapsulation is one of the fundamental concepts in object-oriented programming (OOP). 
It describes the idea of wrapping data and the methods that work on data within one unit.
This puts restrictions on accessing variables and methods directly and can prevent the 
accidental modification of data. To prevent accidental change, an object’s variable can 
only be changed by an object’s method. Those types of variables are known as private variables.

```
class Dog:

    def __init__(self, name, age):  
        self.name = name
        self.age = age
        self.food=food

  def __repr__(self):
    return f"Dog: {self.name}, age: {self.age}, food: {self.author}"
    
mg=Dog('German Shephard',3,'meat')

print(mg.name)
print(mg.age)
print(mg.food)

```

## What is Inheritance?

A class's ability to inherit methods and/or characteristics from another class
is known as inheritance.
It refers to defining a new class with little or no modification to an existing class.
The new class is called derived (or child) class and the one from which it inherits is 
called the base (or parent) class.

```
class Animal:  
    def speak(self):  
        print("Animal Speaking")  
#child class Dog inherits the base class Animal  
class Dog(Animal):  
    def bark(self):  
        print("dog barking")  
d = Dog()  
d.bark()  
d.speak()  
```

#### Multi-Level inheritance
Multi-level inheritance is archived when a derived class inherits another derived class.
There is no limit on the number of levels up to which, the multi-level inheritance is 
archived in python.
```
class Animal:  
    def speak(self):  
        print("Animal Speaking")  
#The child class Dog inherits the base class Animal  
class Dog(Animal):  
    def bark(self):  
        print("dog barking")  
#The child class Dogchild inherits another child class Dog  
class DogChild(Dog):  
    def eat(self):  
        print("Eating bread...")  
d = DogChild()  
d.bark()  
d.speak()  
d.eat()  
```

## What is Polymorphism?
Polymorphism refers to a subclass's ability to adapt a method that already exists in its 
superclass to meet its needs.

```
from math
import pi
class square:
    def __init__(self, length):
    self.l = length
def perimeter(self):
    return 4 * (self.l)
def area(self):
    return self.l * self.l
class Circle:
    def __init__(self, radius):
    self.r = radius
def perimeter(self):
    return 2 * pi * self.r
def area(self):
    return pi * self.r * * 2
# Initialize the classes
sqr = square(10)
c1 = Circle(4)
print("Perimeter computed for square: ", sqr.perimeter())
print("Area computed for square: ", sqr.area())
print("Perimeter computed for Circle: ", c1.perimeter())
print("Area computed for Circle: ", c1.area())
```


## Method Overloading
Methods in Python can be called with zero, one, or more parameters. 
This process of calling the same method in different ways is called method 
overloading. It is one of the important concepts in OOP. Two methods cannot
have the same name in Python; hence method overloading is a feature that allows 
the same operator to have different meanings.

```
class Person:
def Hello(self, name=None):
if name is not None:
print('Hello ' + name)
else:
print('Hello ')
# Create instance
obj = Person()
# Call the method
obj.Hello()
# Call the method with a parameter
obj.Hello('Edureka')
```

## Method Overriding

We can provide some specific implementation of the parent class method in our child class. 
When the parent class method is defined in the child class with some specific implementation, 
then the concept is called method overriding.

```
class Animal:  
    def speak(self):  
        print("speaking")  
class Dog(Animal):  
    def speak(self):  
        print("Barking")  
d = Dog()  
d.speak()  
```




    
    
    



 
 
