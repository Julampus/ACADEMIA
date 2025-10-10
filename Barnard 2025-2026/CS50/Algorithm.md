### CS50 Week 3
#CS50 

**Algorithm**
	Step by step instructions on how to do something

**Linear Search** 
	Is array[i] what we are looking for? If yes, hooray! If no, go array[i+1]
	Stops if runs through whole array and returns false
	Worst case (O): ...has to run *n* times
	Best case (Ω): 1 time

**Binary Search**
	Reduces search area by half each search *only if sorted array*
	Starts at midpoint
	Repeat until the (sub)array is size 0
	Cares about:
		Target - what you hope to find
		Start - lower array # - right of middle **if** target is greater than
		End - upper array # - left of middle **if** target is less than
		Middle - (start + end) / 2 
	Worst case (O): logn
	Best case (Ω): 1 time

**Bubble Sort**
	Compares two elements at a time, swaps lower elements from right to left
	Pseudocode:
		Set swap counter to non zero => Reset swap counter to 0 => Swap if needed for each pair => If swap counter after scan == 0,  end
	Worst case (O): n^2
	Best case (Ω): n times
	
**Selection Sort**
	Finds smallest unsorted element and adds it to the end of a sorted list
	Pseudocode:
		Repeat until no unsorted elements remain
		Look for smallest part, swap with the first element of unsorted part
	Worst case (O): n^2
	Best case (Ω):  n^2 times

**Merge Sort**
	An algorithm that uses [[Recursion]]
	Pseudocode:
		Sorts left half of array
		Sorts right half of array
		Merge together
	Worst case (O): n * log(n)
	Best case (Ω):  n * log(n)