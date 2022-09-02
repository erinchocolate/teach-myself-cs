# ☕Java

## What to study - resources I find helpful📚

- Fundamental
  - [Java Tutorial - For Beginners](https://www.youtube.com/watch?v=Yv_4RXyLjL8&t=9868s)
  - [Java Full Course](https://www.youtube.com/watch?v=xk4_1vDrzzo&t=13455s)
  - [Java Programming All-in-One Tutorial Series](https://www.youtube.com/watch?v=r3GGV2TG_vw&t=22611s)

## Project  - what I do to study the topic⌨️

- [swen501](https://github.com/erinchocolate/swen501)
- [swen502](https://github.com/erinchocolate/swen502)
- [cs61b](https://github.com/erinchocolate/cs61b)

## Study Note ✍️

- [Fundamental](#Fundamental)
- [Advanced](#Advanced)
- [Framework](https://github.com/erinchocolate/teach-myself-cs/blob/master/Programming/Java%20Framework.md)

## Fundamental

Variables

Operators

Argument and Parameters

- arguments - what you pass to a method 
- parameter - variables to store arguments 

Primitive Data Types

- boolean, byte, char, short, long, int, float, double

Conditions

- `if`
- `else if`
- `else`
- `switch`

Loops

- While loop
- Do while loop
- For loop
- For each loop
- `break`
- `continue`

Class and Object

Fields and Methods

Access modifier

- Public
- Private
- Protected

Wrapper class

- Byte, Short, Integer, Long, Float, Double, Boolean, Character

- Provides a way to use primitive data types as reference data types

Constructor

- A constructor method is a special function that creates an instance of the class

Static Methods

- Methods related to the class not object
- The static method is called at class level

Method overloading

- Methods that share the same name but have different parameters

Method overriding

- Subclass provides the specific implementation of the method that has been declared by one of its parent class

Interface

- An `interface` is a completely "**abstract class**" that is used to group related methods with empty bodies

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

- `try` 
- `catch`
- `finally`
- `throw`

File class

Scanner class

PrintStream class

## Advanced

Lambda

Comparator vs Comparable

- [Comparable vs Comparator in Java](https://www.youtube.com/watch?v=oAp4GYprVHM)

Generics

- Enable types to be parameters when defining: classes, interfaces and methods
- A benefit is to eliminate the need to create multiple versions of methods or classes for various data types. Use one version for all reference data types
- Bounded type: you can create the objects of a generic class to have data of specific derived types
- [Generics In Java - Full Simple Tutorial](https://www.youtube.com/watch?v=K1iu1kXkVoA)

`this` keyword

- Refer to the current object
- Inside the constructor method to call another constructor method
- [This Keyword in Java Full Tutorial - How to Use "this"](https://www.youtube.com/watch?v=ETLHbHenW44)

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

Pass Reference v.s Value

- Java is always pass by value, not pass by reference
- [Is Java "pass-by-reference" or "pass-by-value"?](https://stackoverflow.com/questions/40480/is-java-pass-by-reference-or-pass-by-value)

How Java works behind the scene

- JVM
- Garbage collection
- Memory management

Threads

Multiprocessing

Streams

Serialization

Collection framework
- ![Collection](https://github.com/erinchocolate/teach-myself-programming/blob/master/Programming/Images/Collections-in-Java.png)
