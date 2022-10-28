# ☕Java

## Project  - what I do to study the topic⌨️

- [swen501](https://github.com/erinchocolate/swen501)
- [swen502](https://github.com/erinchocolate/swen502)

## Study note  - what I need to know about the topic✍️

### Fundamental

Basic Syntax

Variables

Operators

Data Types

Conditions

Loops

Class and Object

Fields and Methods

Access modifier

Wrapper class

Constructor

Static Methods

Method overloading

- Methods that share the same name but have different parameters

Method overriding

- Subclass provides the specific implementation of the method that has been declared by one of its parent class

Interface

Abstract class and method

- Abstract class is a restricted class that cannot be used to create objects (to access it, it must be inherited from another class)

- Abstract method can only be used in an abstract class, and it does not have a body. The body is provided by the subclass (inherited from)

Interface v.s Abstract class

- You can implement many interface but can only extend one class

- Any fields declared in interface is static and final

Final class, method and variable

- Final class can not be inherited from

- Final method can not be overridden

- Final variable's value can not be changed

Enums

- An enum is a special "class" that represents a group of constants (unchangeable variables, like final variables)

Inner Class

- The purpose of nested classes is to group classes that belong together, which makes your code more readable and maintainable

- To access the inner class, create an object of the outer class, and then create an object of the inner class

Exception handle

File class

Scanner class

PrintStream class

Collection framework

Generics

- Enable types to be parameters when defining: classes, interfaces and methods
- A benefit is to eliminate the need to create multiple versions of methods or classes for various data types. Use one version for all reference data types
- Bounded type: you can create the objects of a generic class to have data of specific derived types

`this` keyword

- Refer to the current object
- Inside the constructor method to call another constructor method

OOP

- Abstraction
- Encapsulation
  - Attributes of a class will be hidden or private. Can be accessed only through methods. You should make attributes private if you don’t have reason to make them public or protected.
  - Getter and setter
- Inheritance
  - `super`
- Polymorphism
  - First type: child class overrides parent class’s method
  - Second type: method overloading

### Dive Deep

Comparator vs Comparable

Pass Reference v.s Value

- Java is always pass by value, not pass by reference

How Java works behind the scene

- JVM
- Garbage collection
- Memory management

Threads

Multiprocessing

Serialization

Lambda
