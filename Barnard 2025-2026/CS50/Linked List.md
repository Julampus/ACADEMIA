#CS50 
###### Linked List - See [[Structs & Nodes]]
Non contiguous list, connected only via. [[Pointers]]
- Also one pointer added to point to "head" of list
	Can lead to "*fragmentation*" of memory on older systems 
Spending **space**, gaining **flexibility**

==Definition of Node:==
```
typedef struct node
{
	int number;
	struct node \*next;
} node;
```

==Example (Built Backwards):== 
```
int main(void)
{
	node \*n = malloc(sizeof(node));
	for (int i = 0; i < size; i++)
	{
		if (n == NULL)
		{
			return 1;
		}
		n->number = get_int("Number: ");
		n->next = list;
		list = n;
	}
	node \*ptr = list;
	while (ptr  != NULL)
	{
		printf("%i\n", ptr ->n)
	}
}
```

==Example (Built Forwards):== 
```
int main(void)
{
	node \*n = malloc(sizeof(node));
	for (int i = 0; i < size; i++)
	{
		if (n == NULL)
		{
			list = n;
		}
		else
		{
			for (node \*ptr = list; ptr != NULL; ptr = ptr-> mext)
			{
				if  (ptr->next == NULL)
				{
				ptr->next = n;
				break;
				}
			}
		}
	}
	for (node \*ptr = list; ptr != NULL; ptr = ptr-> next)
	{
		printf("%i\n", ptr ->number)
	}
	return 0;
}
```

==After printing, how to free:==
```
while (ptr != NULL)
{
	node \*next = ptr->next;
	free(ptr);
	ptr = next;
}
```