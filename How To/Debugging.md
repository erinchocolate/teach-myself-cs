# Debugging

## What to study - resources I find helpful📚

Overview

- [Debugging Guide](https://sp21.datastructur.es/materials/guides/debugging-guide.html)
- [Debugging and Profiling](https://missing.csail.mit.edu/2020/debugging-profiling/)
- [Debugging Checklist - How To Debug Anything](https://www.youtube.com/watch?v=e_kogQ1r9u0)
- [5 Debugging Tips Every Developer Should Know](https://www.youtube.com/watch?v=K6WGRBhacq8)

Debugger

- [How to Use a Debugger - Debugger Tutorial](https://www.youtube.com/watch?v=7qZBwhSlfOo)
- [How To Debug Java Code The Right Way - Eclipse Debugger Full Tutorial](https://www.youtube.com/watch?v=aqcJsKdjjvU&t=436s)

## Study Note ✍️

Print debugging

- A first approach to debug a program is to add print statements around where you have detected the problem, and keep iterating until you have extracted enough information to understand what is responsible for the issue.

Logging

Understanding the stack trace

Debugger

- Break points
- Step over
  - This allows you to execute the current line of code and move on to the next line in this frame.
- Step Into
  - This allows you to step into any function calls in the current line given the functions are yours.
- Step Out
  - If you are in a function or loop, this allows you to skip the rest of the frame, essentially bringing you out to wherever this function was called.

