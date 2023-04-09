# Pointers-c

The pointer in C language is a variable which stores the address of another variable. This variable can be of type int, char, array, function, or any other pointer. The size of the pointer depends on the architecture. However, in 32-bit architecture the size of a pointer is 2 byte.

Consider the following example to define a pointer which stores the address of an integer.

int n = 10;   

int* p = &n;       // Variable p of type pointer is pointing to the address of the variable n of type integer.   


Declaration of Pointer:

Syntax: Datatype *ptr_name;

Example: int *p;

Here, the * mark before the variable indicates that it is a pointer variable. Indirection operators must be required between datatype and variable name. Space is not mandatory to place in the declaration of the pointer variable.


Initialization of Pointer:

Syntax:
Datatype variable;

Datatype *ptr = &variable;



Pointer to array

int arr[10];  
int *p[10]=&arr; // Variable p of type pointer is pointing to the address of an integer array arr.  

Pointer to a function

void show (int);  
void(*p)(int) = &display; // Pointer p is pointing to the address of a function  

Pointer to structure

struct st {  
    int i;  
    float f;  
}ref;  
struct st *p = &ref;  


NULL Pointer

A pointer that is not assigned any value but NULL is known as the NULL pointer. If you don't have any address to be specified in the pointer at the time of declaration, you can assign NULL value. It will provide a better approach.

int *p=NULL;

Generic Pointers
A generic pointer is a pointer variable that has void as its data type. The void pointer, or the generic pointer, is a special type of pointer that can point
to variables of any data type. It is declared like a normal pointer variable but using the void keyword as the
pointer’s data type.
Eg. void *ptr;

In C, since you cannot have a variable of type void, the void pointer will
therefore not point to any data and, thus, cannot be dereferenced. Generic pointers are often used when you want a pointer to point to data of different types at different times.
