# Class Six Reading

## Explain the difference between an object and a class

Object: An object is a tangible instance of a class. It is a self-contained unit that encapsulates both data (attributes) and behaviors (methods).

Class: A class is a blueprint or a template for creating objects. It defines the structure, attributes, and methods that the objects created from it will possess. 

## Explain to a non-technical friend the concept of inheritance in Java

Imagine you're building a virtual zoo in a computer program. You want to create different kinds of animals, like lions, tigers, and bears. Now, instead of writing all the code for each animal from scratch, you can use something called "inheritance" in Java. Inheritance is like passing down traits in a family. So, in our zoo example, you can create a "Parent Animal" with all the basic features that animals share, like their name, age, and the ability to make sounds. Then, when you want to make specific animals like lions or tigers, you can create "Child Animals" that inherit everything from the "Parent Animal," like their name, age, and sound-making ability. But these child animals can also have their own unique features.

## Static methods are also called what? Why?

Static methods are also called "class methods." They are called so because they belong to the class itself rather than to any specific instance or object of that class

## How can you access a variable of a class without instantiating an object from that class?

You can do that by using a static variable. Static variables are associated with the class itself rather than with individual instances of the class, so they can be accessed directly using the class name.

## What is a Design Pattern? Describe one or two with analogies from your previous work experience

A design pattern is a reusable and proven solution to a common software design problem. It's like a blueprint or template that provides a structured way to solve recurring design challenges in software development.

Two analogies:

- Singleton Pattern
- Observer Pattern

## What is a Singleton?

It is a  design patterns that ensures that a class has only one instance and provides a global point of access to that instance, much like the receptionist handling all printer interactions. This is useful for scenarios where you want to limit the creation of instances to avoid conflicts, such as managing a single database connection throughout an application.