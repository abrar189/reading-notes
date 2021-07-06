# Functional Programming Concepts

1. What is functional programming?

In computer science, functional programming is a programming paradigm where programs are constructed by applying and composing functions. It is a declarative programming paradigm in which function definitions are trees of expressions that map values to other values, rather than a sequence of imperative statements which update the running state of the program.

2. What is a pure function and how do we know if something is a pure function?

Pure Functions A pure function is a function which: Given the same input, will always return the same output. Produces no side effects

3. What are the benefits of a pure function? Benefits of pure functions: They’re easier to reason about

- combine
- test
- debug
- parallelize

4. What is immutability?

Immutables are the objects whose state cannot be changed once the object is created. Strings and Numbers are Immutable.
What is Referential transparency? Referential transparency and referential opacity are properties of parts of computer programs. An expression is called referentially transparent if it can be replaced with its corresponding value (and vice-versa) without changing the program’s behavior.

# Node JS Tutorial for Beginners #6 - Modules and require()

1. What are JS modules? J

S modules (also known as “ES modules” or “ECMAScript modules”) are a major new feature, or rather a collection of new features. You may have used a userland JavaScript module system in the past.

2. What does the word ‘require’ do? 

require() is used to consume modules. It allows you to include modules in your app.

3. What do we have to do to make a module available? 

The first thing you do to get access to module features is export them. This is done using the export statement.