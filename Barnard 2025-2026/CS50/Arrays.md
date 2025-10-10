### CS50 Week 5 (Week 3 Concept)
#CS50 

**Arrays** - Contiguous linkage of different values, ending in NUL
%% Example[](String.md)]]s in CS50

**To declare an Array** - 
Code "*what type located within array*" *varb_name*[Size]

**Growing an Array** - Issue is, might be bleeding into real or garbage values
Perchance can *swap* into garbage values
***!*** - Issue, takes time

**Can also make an array like:**
int \*list = malloc(3 * sizeof(int));
%% See realloc in [[Memory]] %%
%% "There's always a tradeoff between time and space" %%