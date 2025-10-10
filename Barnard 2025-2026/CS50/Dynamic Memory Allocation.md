### CS50 Week 4
#CS50 
Extension of [[Memory]]

- All memory that needs to be used is set up in a **static** (from the *stack*) setup (difficult if you want any memory flexibility)

**DMA** - Getting new memory (from the *heap*) while the program is running 
	You can do this by using Malloc
**Memory leak** occurs when  you don't use the *free()* function

Note: the *heap* grows down in memory section while the *stack* grows up (***shared space***)