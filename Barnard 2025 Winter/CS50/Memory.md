### CS50 Week 4
#CS50 
%% Work and change performed in RAM, referred to in [[Hexadecimal]]  %% 

**Memory** - part of ==<stdlib.h>==
- *malloc(sizeof[type_n])* command = creates new chunk of n bytes of memory (See: [[Dynamic Memory Allocation]])
	Returns address ***&*** of first byte
		See [[Pointers]]
	In cases of error, returns NULL (so, check for NULL)
- *free(adress_n)* command "does the opposite" = gives memory back from whichever address is associated (from malloc)
- *realloc(**adress_of_memory_to_resize*, new size)** - for growing memory
	- Still need to free

- use **valgrind** *./code* command line function to look for memory leaks
- *swap(x, y)*, creates swap memory, swaps the address of the two variables
	must be within scope, else x and y are ==*passed by value*== within its own function
	instead, *==pass by reference==*, swapping the [[Pointers]] and **addresses** rather than the variables
	
	in other words, within its own frame on a [[Call Stack]]

%% Training wheels are off! %%