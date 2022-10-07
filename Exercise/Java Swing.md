# Java Swing

## What to study - resources I find helpful📚

- [Java Swing](https://www.youtube.com/watch?v=Kmgo00avvEw&t=1992s)

## Project  - what I do to study the topic⌨️

- 

## Study Note ✍️

JFrame

- a **JFrame** represents a framed window

JPanel

- **JPanel** represents some area in which controls (e.g., buttons, checkboxes, and textfields) and visuals (e.g., figures, pictures, and even text) can appear
- Once we write a **JFrame** for our GUI, we often add one or more objects to it, each from a subclass extending **JPanel**. 

paintComponent method

- The **paintComponent** method determines what figures, images, and/or text (controls like buttons and textfields are painted automatically) appear on the part of the screen that is owned by the **JPanel**

Graphics class

- Whenever the **paintComponent** method of a **JPanel** is called (whether by the Java system or the program itself), it is supplied with a reference to an object from the **Graphics** class (called its graphics context). 

Action Listener

- ActionListener in Java is a class that is responsible for handling all action events such as when the user clicks on a component. Mostly, action listeners are used for JButtons.

How to write an Action Listener

- Declare an event handler class and specify that the class either implements an ActionListener interface or extends a class that implements an ActionListener interface. For example:

  - ```java
    public class MyClass implements ActionListener { 
    ```

- Register an instance of the event handler class as a listener on one or more components. For example:

  - ```java
     someComponent.addActionListener(instanceOfMyClass);
    ```

- Include code that implements the methods in listener interface. For example:

  - ```java
     public void actionPerformed(ActionEvent e) { 
            ...//code that reacts to the action... 
        }
    ```

Key Listener

- The listener interface for receiving keyboard events (keystrokes). 
- The class that is interested in processing a keyboard event either implements this interface (and all the methods it contains) or extends the abstract `KeyAdapter` class (overriding only the methods of interest).