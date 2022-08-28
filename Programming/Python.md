# 🐍Python

## What to study - resources I find helpful📚

- Fundamental
  - [Computational Thinking using Python](https://www.edx.org/xseries/mitx-computational-thinking-using-python)
  - [Python Tutorials](https://www.youtube.com/playlist?list=PL-osiE80TeTt2d9bfVyTiXJA-UTHn6WwU)
  - [Intermediate Python Tutorials](https://www.youtube.com/playlist?list=PLzMcBGfZo4-nhWva-6OVh1yKWHBs4o_tv)
- Advanced
  - [Python Tips](https://book.pythontips.com/en/latest/index.html)
  - [Expert Python Tutorials](https://www.youtube.com/watch?v=mclfteWlT2Q&list=PLzMcBGfZo4-kwmIcMDdXSuy_wSqtU-xDP)
  - [Python Classes & Objects Tutorial](https://www.youtube.com/watch?v=v_Jp11xqCzg&list=PLzMcBGfZo4-l1MqB1zoYfqzlj_HH-ZzXt)
  - [Python Object-Oriented Tutorials](https://www.youtube.com/playlist?list=PL-osiE80TeTsqhIuOqKhwlXsIBIdSeYtc)

## Project  - what I do to study the topic⌨️

- [python-exercise](https://github.com/erinchocolate/python-exercise)

## Study Note ✍️

- [Fundamental](#Fundamental)
- [Advanced](#Advanced)
- [Standard Library](#Standard-Library)
- [Framework]()



## Fundamental

Variable

- Naming
- Scope

Data types

Operators

Conditions

- `If`
- `elif`
- `else`

Function

- `return`
- `global`

Loops

- While loop
- For loop
- `break`
- `continue`

Exception

- `try`
- `except`
- `raise`
- `finally`

File object

- Read
- Write

Data Structures

- List	

  - Ordered

  - Changeable

  - Allow Duplicates


- Dictionary

  - Ordered after python 3.7

  - Changeable

  - Duplicates Not Allowed


- Set

  - Unordered

  - Unchangeable

  - Duplicates Not Allowed


- Tuple

  - Ordered

  - Unchangeable

  - Allow Duplicates

Iterators

- Iterable
  - Any object which has methods:
    - `__iter__`
    - `__getitem__`
  - In short an `iterable` is any object which can provide us with an **iterator**.
- Iterator
  - Any object which has methods:
  - `__next__`
- Iteration
  - When we use a loop to loop over something it is called iteration

Generators

- Generators are iterators, but you can only iterate over them once

- Generators do not store all the values in memory, they generate the values on the fly

  - `yield`

  - [Python Generators Explained](https://www.youtube.com/watch?v=u3T7hmLthUU)


## Advanced

args and kwargs

Collections

- `defaultdict`
- `OrderedDict`
- `Counter`
- `deque`
- `namedtuple`
- `enum.Enum`

Enumerate

- It allows us to loop over something and have an automatic counter

Zip and unzip

- Zip is a useful function that allows you to combine two lists easily

Object introspection

- introspection is the ability to determine the type of an object at runtime
- `dir`
- `type`
- `id`
- `inspect` module

Comprehensions

- Comprehensions are constructs that allow sequences to be built from other sequences

  - list comprehensions

    - ```python
      variable = [out_exp for out_exp in input_list if out_exp == 2]
      ```

  - dictionary comprehensions

    - ```python
      {v: k for k, v in some_dict.items()}
      ```

  - set comprehensions

    - ```python
      squared = {x**2 for x in [1, 1, 2]}
      print(squared)
      # Output: {1, 4}
      ```

  - generator comprehensions

    - ```python
      multiples_gen = (i for i in range(30) if i % 3 == 0)
      print(multiples_gen)
      # Output: <generator object <genexpr> at 0x7fdaa8e407d8>
      for x in multiples_gen:	
        print(x)
        # Outputs numbers
      ```

OOP

- Classes and objects
- Class methods and object methods
- Magic methods
- Inheritance

Decorators

- they are functions which modify the functionality of other function

Context manager

- `with`

- [Python Tutorial: Context Managers - Efficiently Managing Resources](https://www.youtube.com/watch?v=-aKFBoZpiqA&list=PL-osiE80TeTt2d9bfVyTiXJA-UTHn6WwU&index=50)

For/else loop

- ```python
  for item in container:
      if search_something(item):
          # Found it!
          process(item)
          break
  else:
      # Didn't find anything..
      not_found_in_container()
  ```

Lambda 

- small anonymous function

  - ```python
    add = lambda x, y: x + y
    
    print(add(3, 5))
    # Output: 8
    ```

String formatting

- format()
- f string
  - [Python Quick Tip: F-Strings - How to Use Them and Advanced String Formatting](https://www.youtube.com/watch?v=nghuHvKLhJA&list=PL-osiE80TeTt2d9bfVyTiXJA-UTHn6WwU&index=36)


Clean code

- Pep8 is a styleguide for python

- [Write Python Code Properly](https://www.youtube.com/watch?v=D4_s3q038I0&t=13s)

Virtual Environment

- make isolated python environments
- virtualenv
  - [Python Tutorial: virtualenv and why you should use virtual environments](https://www.youtube.com/watch?v=N5vscPTWKOk&list=PL-osiE80TeTt2d9bfVyTiXJA-UTHn6WwU&index=15)
- pipenv
  - [Python Tutorial: Pipenv - Easily Manage Packages and Virtual Environments](https://www.youtube.com/watch?v=zDYL22QNiWk&list=PL-osiE80TeTt2d9bfVyTiXJA-UTHn6WwU&index=59)
- venv
  - [Python Tutorial: VENV (Windows) - How to Use Virtual Environments with the Built-In venv Module](https://www.youtube.com/watch?v=APOPm01BVrk&list=PL-osiE80TeTt2d9bfVyTiXJA-UTHn6WwU&index=107)

## Standard Library

Pip

- [Python Tutorial: pip - An in-depth look at the package management system](https://www.youtube.com/watch?v=U2ZN104hIcc)

Logging

- [Python Tutorial: Logging Basics - Logging to Files, Setting Levels, and Formatting](https://www.youtube.com/watch?v=-ARI4Cz-awo&list=PL-osiE80TeTt2d9bfVyTiXJA-UTHn6WwU&index=54)
- [Python Tutorial: Logging Advanced - Loggers, Handlers, and Formatters](https://www.youtube.com/watch?v=jxmzY9soFXg)

Unit testing

- [Python Tutorial: Unit Testing Your Code with the unittest Module](https://www.youtube.com/watch?v=6tNS--WetLI&list=PL-osiE80TeTt2d9bfVyTiXJA-UTHn6WwU&index=58)

Threading

- [Python Threading Tutorial: Run Code Concurrently Using the Threading Module](https://www.youtube.com/watch?v=IEEhzQoKtQU)

Multiprocessing

- [Python Multiprocessing Tutorial: Run Code in Parallel Using the Multiprocessing Module](https://www.youtube.com/watch?v=fKl2JW_qrso&list=PL-osiE80TeTt2d9bfVyTiXJA-UTHn6WwU&index=126)

Regular Expression

- [Python Tutorial: re Module - How to Write and Match Regular Expressions (Regex)](https://www.youtube.com/watch?v=K8L6KVGG-7o&list=PL-osiE80TeTt2d9bfVyTiXJA-UTHn6WwU&index=31)

Subprocess

- [Python Tutorial: Calling External Commands Using the Subprocess Module](https://www.youtube.com/watch?v=2Fp1N6dof0Y&list=PL-osiE80TeTt2d9bfVyTiXJA-UTHn6WwU&index=123)

Json

- [Python Tutorial: Working with JSON Data using the json Module](https://www.youtube.com/watch?v=9N6a-VLBa2I&list=PL-osiE80TeTt2d9bfVyTiXJA-UTHn6WwU&index=48)

CSV

- [Python Tutorial: CSV Module - How to Read, Parse, and Write CSV Files](https://www.youtube.com/watch?v=q5uM4VKywbA&list=PL-osiE80TeTt2d9bfVyTiXJA-UTHn6WwU&index=29)

Operating System

- [Python Tutorial: OS Module - Use Underlying Operating System Functionality](https://www.youtube.com/watch?v=tJxcKyFMTGo&list=PL-osiE80TeTt2d9bfVyTiXJA-UTHn6WwU&index=24)

Asynchronous Programming

- [Python Asynchronous Programming - AsyncIO & Async/Await](https://www.youtube.com/watch?v=t5Bo1Je9EmE)
