# 🔢What is Data Structure

## Study Note ✍️

### What is data structure

- A data structure is a way of organizing data so that it can be used effectively

### What is Abstract Data Type

- An abstract data type is an abstraction of a data structure which provides only the interface to which a data structure must adhere to
- The interface does not give any specific details about how something should be implemented or in what programming language
- ![Common ADT](https://github.com/erinchocolate/teach-myself-cs/blob/master/Data%20Structure%26Algorithm/Images/Common%20ADT.png)

### ADT v.s CDT

- Abstract Data Type(ADT) is a data type, where only behavior is defined but not implementation
- Opposite of ADT is Concrete Data Type (CDT), where it contains an implementation of ADT
- Array, List, Map, Queue, Set, Stack, Table, Tree, and Vector are ADTs. Each of these ADTs has many implementations i.e. CDT
- ![ADT](https://github.com/erinchocolate/teach-myself-cs/blob/master/Data%20Structure%26Algorithm/Images/ADT.png)
- ![ADT V.S DS](https://github.com/erinchocolate/teach-myself-cs/blob/master/Data%20Structure%26Algorithm/Images/ADT%20v.s%20DS.png)

### Array v.s Linked List

- There are only two ways to store data structures: as arrays (sequential storage) or as linked lists (linked storage)
- Other data structures can be viewed as special operations on linked lists or arrays
  - 「queue」 and 「stack」 data structures can be implemented with both linked lists and arrays
  - A graph can be implemented with both linked lists and arrays. An adjacency table is a linked list, and an adjacency matrix is a two-dimensional array

### Operations on data structure

- For any data structure, its basic operation is no more than traversal + access, and more specific point are: add, delete, search and modify
- There are many kinds of data structures, but their purpose is to add, delete, search and modify them as efficiently as possible in different application scenarios
- How to traverse + access? Two forms: linear and nonlinear
