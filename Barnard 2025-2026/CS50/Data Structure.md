### CS50 Week 5
%% See [[Structs & Nodes]] for syntax in declaring data types %%
#CS50 
###### Queues
Ordering in a line
Example of a *FIFO* (First in First Out) type
*Enqueue* - to put something into tfhe queue
*Dequeue* - to take something out of the queue

==Example in C:==
```
const int CAPACITY = 50;

typedef struct
{
	person people[CAPACITY];
	int size;
} queue;
```
###### Stacks
The last object you put in is the first you take out
Array-based (by default)
%% See [[Call Stack]] for order of opporations of functions in C %%
*Example*: a stack of clothes, not getting to the sweater at the bottom
This is an example of *LIFO* (Last in First Out [Opposite of *FIFO*]
*Push* - means to push on top of stack
*Pop* - remove something from top of the stack

==Example in C:==
```
const int CAPACITY = 50;
typedef struct
{
	person people[CAPACITY];
	int size;
} stack;
```

%% Differs from *FIFO* in the operations that control the stuct %%
###### Linked List
**Rather than using [[Arrays]] with Back-to-Back memory, why not use pointers?**
Need:
	struct
	. (dot operator)
	*+*
	\* (deference operator)
	*=*
	-> (arrow operator) 
	%% See [[Linked List]] %%
	
Can be achieved using [[Dynamic Memory Allocation]] (Malloc)

*Singly Linked Lists* - One Way [[Pointers]]
*Doubly Linked Lists* - Two Way [[Pointers]]

###### Tree (The goat)
2D data structure - binary search tree
Code using [[Recursion]] to search the tree
```
typedef struct node
{
	int number;
	struct node *left;
	struct node *right;
} node;
```
###### Dictionary / HashTable
split into words/keys and definitions/values
can be strings, numbers, etc...

The question is, *can we achieve **constant** time?*
Still ***O(n/k)***  :(

**Hashing** - Hash function takes input, produces output
**Bucketizing** - Putting an input into its own location (a. la. sorting a deck of cards in suit and number order)
Issue with **Collision** (Two+ things in the same bucket) => Solve with a [[Linked List]]

==Example in C:==
```
typedef struct node
{
	int number;
	char *name;
	char *number;
	struct node *next;
} node;
```

###### Tries
a **Tree** of [[Arrays]]
Following an array for each letter (in a persons name...) with size 26 for each
Toad v.s. Toadette, can keep following the pointers
Using **Terminal** points to show "Name ends here"
***O(1)*** = *CONSTANT TIME* (at the cost of memory)

==Example in C:==
```
typedef struct node
{
	struct node *children[26];
	char *number;
} node;
```