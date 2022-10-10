# 🔢Analysis of Algorithm

## What to study - resources I find helpful📚

- [Runtime Complexity Explained](https://www.youtube.com/watch?v=zfrz0XEuqA4&list=PL7yh-TELLS1HgoWUfxGzoaa7PEJ2Q-RfC&index=4)

- [Analysis of Algorithms](https://algs4.cs.princeton.edu/14analysis/)
- [Big O Notation & Time Complexity Analysis Tutorial](https://www.youtube.com/watch?v=6aDHWSNKlVw&t=28s)

## Study Note ✍️

### How to determine efficiency of a program?

- Memory
- Runtime

### How to calculate runtime?

- Calculate primitive operations

  - cost model: sum of cost * frequency for all operations

    - Need to analyze program to determine set of operations

    - Frequency depends on algorithm, input data

- Focus on the worst case - provides a guarantee for all inputs
- Focus on the asymptotic growth - suppress details in analysis

### Order-of-Growth

| order of growth | name         | typical code framework                 | description        | example           |
| --------------- | ------------ | -------------------------------------- | ------------------ | ----------------- |
| 1               | constant     | a = b + c                              | statement          | add two numbers   |
| logN            | logarithmic  | while (N>1){N = N/2...}                | divide in half     | binary search     |
| N               | linear       | for (int i = 0; i < N; i++){<br />...} | loop               | find the maximum  |
| NlogN           | linearithmic | merge sort                             | divide and conquer | merge sort        |
| N^2             | quadratic    |                                        | double loop        | check all pairs   |
| N^3             | cubic        |                                        | triple loop        | check all triples |
| 2^N             | exponential  |                                        | exhaustive search  | check all subsets |

### Common notations

- Big Theta - classify algorithms
- Big O - develop upper bounds
- Big Omega - develop lower bounds