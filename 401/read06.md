# Inheritance and Interfaces

## Object

- An object is a software bundle of related state and behavior. Software objects are often used to model the real-world objects that you find in everyday life. This lesson explains how state and behavior are represented within an object, introduces the concept of data encapsulation, and explains the benefits of 
designing your software in this manner.

## Class

- A class is a blueprint or prototype from which objects are created. This section defines a class that models the state and behavior of a real-world object. It intentionally focuses on the basics, showing how even a simple class can cleanly model state and behavior.

## Inheritance

- explains how classes inherit state and behavior from their superclasses, and explains how to derive one class from another using the simple syntax provided by the Java programming language

- Object-oriented programming allows classes to inherit commonly used state and behavior from other classes.

- In the Java programming language, each class is allowed to have one direct superclass, and each superclass has the potential for an unlimited number of subclasses.

## Interfaces in Java

In the Java programming language, an interface is a reference type, similar to a class, that can contain only constants, method signatures, default methods, static methods, and nested types. Method bodies exist only for default methods and static methods. Interfaces cannot be instantiated—they can only be implemented by classes or extended by other interfaces

## What You Can Do in a Subclass

1. The inherited fields can be used directly, just like any other fields.
2. You can declare a field in the subclass with the same name as the one in the superclass, thus hiding it (not recommended).
3. You can declare new fields in the subclass that are not in the superclass.
The inherited methods can be used directly as they are.
4. You can write a new instance method in the subclass that has the same signature as the one in the superclass, thus overriding it.
5. You can write a new static method in the subclass that has the same signature as the one in the superclass, thus hiding it.
6. You can declare new methods in the subclass that are not in the superclass.
7. You can write a subclass constructor that invokes the constructor of the superclass, either implicitly or by using the keyword super.

## Private Members in a Superclass

A subclass does not inherit the private members of its parent class. However, if the superclass has public or protected methods for accessing its private fields, these can also be used by the subclass.
