### CS50 Week 3
#CS50

**Recursive Function** 
	A function that *calls itself* based on an [[Algorithm]]
	Runs over and over, n times, and iterates upon itself
	e.g. factorial function n!
		fact(n) = n * fact(n-1)
	Sets aside function as active frame in [[Call Stack]]

requires at least one **base case** that stops the recursion 
	for the factorial example, fact(1) = 1
	
**base case** is called first as an *if* statement 
	if (n == 1) ... **base case**
**recursion** is called as *else* statement
	else ... **recursion**