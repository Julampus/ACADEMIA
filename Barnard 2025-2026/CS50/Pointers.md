### CS50 Week 4
#CS50 

**Pointer** - a variable that stores the address of something 
	***&*** is an address, or *address operator* 
	***\**** is how to get there, *dereference operator*
		means "<u>go to address</u>" / establishes some int as a pointer
	*%p* is a pointer
	*e.g:*
		int n = 50;
		int \*p = &n
		%% Some variable p, pointer, assigned to the address n and deferred as an integer %%
		printf("%p\n", p);
		%% Prints the address of the pointed integer in [[Hexadecimal]] %%
	Addresses change in memory
If you don't set a pointer to anything, set it to **Null**
	Causes a segmentation fault (better than potentially damaging memory for another program)
	
