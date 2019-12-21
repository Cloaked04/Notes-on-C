# Notes-on-C
This repository contains notes on C. No particular order. Recorded as encountered.
-------------------------------------------------------------------------------------------------------------------------------
**Pointers:**<\br>
--> We can change the value of pointer and we can also change the value of object pointer pointing to. Pointer and value pointed by pointer both are stored in the read-write area. 

--> When using the *Const* qualifier, the value cannot be changed for generally, the value is places in the read-only portion of the memory. 

--> When the pointer is a constant, we can change the object/ location the pointer is pointing to but can't change the value of the location using pointer.

--> If say a pointer is const and a variable is not, it the variable will be upqualified to const and then the value can be assigned to a const pointer. But if a const variable can't be pointed to a pointer that has both read-write priviledges as this might allow to change the value of the const variable via the pointer. This can lead to multiple unwanted errors and failures.

--> If a pointer is flagged as a const, it cannot be assigned to a new location, but allows change of value to the object it is pointing to. 

--> If constant pointer is assigned to a constant variable like *const int /*const ptr;* or other ways when the pointer is const and the var is also const, similar things will happen --- the value can't be changed, neither it can be pointed to a new variable/location.

Examples at: https://www.geeksforgeeks.org/const-qualifier-in-c/  </br>

Link for string/ char pointers: https://www.geeksforgeeks.org/whats-difference-between-char-s-and-char-s-in-c/ </br>

Double stars on char represent address to the pointer to char*(the array).[If confused here, above link will definitely help.]

</br></br>

**Typedef:** Assigns name to an already defined data type. Now this new name can be used to declare variables of this type. Syntax: *typedef datatype_name new_name*. <\br> It has different sytax if used for struct. The new name is written just after closing braces of struct.<\br> If a pointer syntax like * int* x* is assigned as pointer like *typedef int* ptr_maker*, then any number of pointers can be made using this new name. 

