# 🐍Python

## Project  - what I do to study the topic⌨️

- [python-exercise](https://github.com/erinchocolate/python-exercise)

## Study note  - what I need to know about the topic✍️

### Fundamental

Variable

Data types

Operators

Conditions

Function

Loops

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

### Dive Deep

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


Clean code

- Pep8 is a styleguide for python

Virtual Environment

- make isolated python environments
- virtualenv
- pipenv
- venv

### Standard Library

Pip

Logging

Unit testing

Threading

Multiprocessing

Regular Expression

Subprocess

Json

CSV 

OS module

Asynchronous Programming
