# Debugging

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

