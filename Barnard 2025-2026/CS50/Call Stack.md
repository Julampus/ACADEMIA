### CS50 Week 3
#CS50

If function (**frame**) called, space will be made to store values and space to store functions in ram 

Multiple functions can exist in memory, called **open frames** because they cannot all be active at once

Most recent frame (that is currently active) at top of stack is called the **active frame**

When a new frame is called, it becomes the **active frame**

In [[Memory]], the stack moves up from the "bottom" (as opposed to the *heap*)

When a function is done, its "**popped off**" of the stack