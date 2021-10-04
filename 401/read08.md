# OO Design

## SOLID principles intro

- Single-responsibility Concept This principle argues that a class should have just one cause to change, or in other words, a single task .

- SOLID is a structured design approach that ensures your software is modular and easy to maintain, understand, debug, and refactor.

- Principle of Interface Segregation This concept asserts that customers should never be compelled to implement an interface that they do not use, or to rely on methods that they do not utilize.

- The Principle of Dependency Inversion Entities must rely on abstractions rather than concretions, according to this concept. It specifies that the high-level module should rely on abstractions rather than the low-level module. Decoupling is also possible as a result of this.

## SOLID: The First 5 Principles of Object Oriented Design:

1. Single-Responsibility Principle (SRP):
A class should have one and only one reason to change, meaning that a class should have only one job.

For example, consider an application that takes a collection of shapes—circles, and squares—and calculates the sum of the area of all the shapes in the collection.

2. Open-Closed Principle:
Objects or entities should be open for extension but closed for modification. This means that a class should be extendable without modifying the class itself.

3. Liskov Substitution Principle:
Let q(x) be a property provable about objects of x of type T. Then q(y) should be provable for objects y of type S where S is a subtype of T. This means that every subclass or derived class should be substitutable for their base or parent class.

4. Interface Segregation Principle:
A client should never be forced to implement an interface that it doesn’t use, or clients shouldn’t be forced to depend on methods they do not use.

5. Dependency Inversion Principle:
Entities must depend on abstractions, not on concretions. It states that the high-level module must not depend on the low-level module, but they should depend on abstractions.