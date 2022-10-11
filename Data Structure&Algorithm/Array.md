# 🔢Array

## My Implementation🧰



## LeetCode✏️



## Study Note ✍️

Overview

- Arrays offer compact and continuous storage, which can be accessed randomly. 
- They make it possible to find elements quickly via index and use storage space efficiently. Because of the need for continuous chunks of memory, sufficient storage space must be allocated at one time. Therefore, if the array has to be expanded, we need to find and reallocate a larger space first, and then copy all the data over; time complexity *O(n)*. 
- And if you want to insert and delete elements in the middle of the array, you must move all the data each time to maintain the continuity; time complexity *O(n)*.

Type

- Static array 
  - a fixed length container containing n elements indexable from the range [0, n-1]
- Dynamic array
  - The dynamic array can grow and shrink in size

Dynamic array

- How to implement dynamic array
  - Create a static array and change the size based on elements
- Advantages
  - random access of elements
  - Good locality of reference and data cache utilization
  - Easy to insert/delete at the end
- Disadvantage
  - Wastes more memory
  - Shifting elements is time consuming O(n)
  - Expanding/shirking the array is time consuming

Complexity
![complexity](https://github.com/erinchocolate/teach-myself-cs/blob/master/Data%20Structure%26Algorithm/Images/array%20complexity.png)
