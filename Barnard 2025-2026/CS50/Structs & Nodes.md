### CS50 Week 3
#CS50 

**Establish a struct:**

```
typedef struct 
{
type 1 *name 1*
type 2 *name 2*
...
type n *name n*
}*name_struct*
```

%% then declare variable with the struct%%

```
*name1* **var_name**;

**var_name**.*name 1* = "input";
**var_name**.*name 2* = "input";
...
**var_name**.*name n* = "input";

*name1*[i].*name n*;
```

works with arrays, too
###### Nodes - [[Data Structure]] for Linked List
%% An example of [[Recursion]] for data structures? %%
```
typedef struct node
{
	int number;
	struct node *next;
} node;
```