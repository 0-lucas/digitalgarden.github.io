# What is it?

*Linked lists* are a linear [[Data Structures|data structure]], very similar to *dynamic [[Arrays]]*. However, *linked lists* work with *non-sequential memory allocation*. This means that the **data is sparsely stored inside memory**, instead of a *sequential allocation*, which happens in [[Arrays]].

This makes *linked lists* offer *memory efficiency* and *scalability*, once it can use any *leftovers* inside memory, and also can **add and remove elements at any position**.
___
# How does it work?

*Linked lists* needs to **store additional information inside each *element***, besides the *element's* actual value. In this case, it stores the *memory address* of other *elements*. 
For example, the *head element* - the first element of a *linked list* - points to the second *element*, which points to the *third*, and so on. The last *element* points to a *null value*.

To find to a *element*, a program **may need to run through** the *linked list* until it finds what it's searching for, which can add [[Algorithm Complexity|time complexity]] to a program.

![[Pasted image 20240611204514.png]]