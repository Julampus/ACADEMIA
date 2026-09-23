### CS50 Week 4
#CS50 

**File I/O** - functions for making files in programs in C
	*fopen("**name for file",  "mode"**)* - opens a file 
	*fclose(**"name for file",  "mode"**)* - closes file
	*fprintf(**"name for file",  "what is to be included"**)* - adds line to specified file
	*fread*(***buffer variable* (where its stored), *size of blocks to read* (bytes),  *how many blocks to read*, *input* (from which file)**) - "reads"/copies data to *buffer* from the [pointer]
		Can use malloc (See [[Memory]]) to create space for buffer
	*fwrite*((***buffer variable* (where its stored), *size of blocks to read* (bytes),  *how many blocks to read*, *output* (to which file)**) - "writes"/adds information from *buffer* to the [pointer]
%% Can use file [[Pointers]] for arguments WITHIN RANGE OF MODE %%


**Modes** - arguments for *File I/O* commands
- *r* - reading (and gathering info from a file)
- *w* - overwriting (if it already exists) or creating a new file with the specified data
- *a* - append... starts from end of existing file and adds data

**New Data-type**
	*FILE* - type for files
	***uint8_t*** - unsigned integer of size: byte (8 bits)