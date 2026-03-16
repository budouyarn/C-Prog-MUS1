# C-Prog-MUSem1
C Programme Practices and Assessment for my Bachelor's Module

During my first semester in Murdoch University, I was made to learn C Programme, compared to what I had learned in Python

Loops
Through my previous beginning practices learning Python coding, I was able to grasp the simple mechanism behind using for loops and while loop

[What is something new in C programme that I learned?]
1) In C Programme, I further learned the exitence of a do while lopp, than just a simple while loop with no existence of an exit, such as  #include<stdbool.h> to use a True False value to control the while loop re-iterations

3) I further explored the usage of Nested loops which can be useful when processing 2D arrays or generating patterns.
   Especially when it comes to swapping of values in order to facilitate linear search functions.

5) Arrays & Dynamic Arrays.
   - Arrays were something lightly touched on in python, where linked list were mostly more utilised back in my practices.
   - I learned so much more in saving input and storing them in an array, which then using functions to manipulate the data.
   - Dynamic arrays were pretty much a new concept to me, where the idea of creating a dynamic array makes flows so much flexiblle by uses allocating memory on the heap using malloc() and calloc().
     
6) Characters and Strings.
   -Using the char data type and understanding ASCII values.
   -Reading and writing individual characters with getchar() / putchar().
   -Working with character arrays (C strings) and the null terminator \0.Using standard library functions from <string.h> such as strlen(), strcpy(), strcmp(), and strcat().
   -Classifying characters using <ctype.h> functions like isalpha(), isdigit(), and toupper().
   
7) Pointers and Addresses.Declaring and initialising pointers using the address-of operator &.	  
    -Dereferencing pointers with * to read and modify values.	  
    -Pointer arithmetic — advancing through arrays by incrementing pointer addresses.	  
    -The relationship between arrays and pointers.	  
    -Passing pointers to functions to enable pass-by-reference behaviour.	  
    -Double pointers (**) for modifying pointer variables inside functions.

8) Functions
-All functions follow a single-responsibility principle: each function does one thing and does it well.
  -Declaring functions with appropriate return types and parameter lists.	  
  -Separating function declaration (prototype) from definition.  
  -Passing arguments by value and by pointer (reference).  
  -Returning values from functions, including returning pointers to heap-allocated data.  
  -Recursive functions — functions that call themselves to solve problems like factorial calculation or binary search.
  


9) Modularity
   -Good C programs are split across multiple files for maintainability and reuse. This project demonstrates modularity through:
   -Header files (.h) — contain function prototypes, constants (#define), and type definitions shared across files.
   -Source files (.c) — contain function implementations, each file grouped by logical responsibility.
   -Include guards — #ifndef / #define / #endif blocks in every header to prevent double inclusion.
   -main.c — serves as the entry point only; all logic is delegated to dedicated modules.


7) Sorting Algorithms
      -Linear Search — explains the sequential scan approach, shows the C implementation with an early return on match, and covers best/worst case complexity (O(1) to O(n)).
      -Bubble Sort — covers the nested-loop comparison-and-swap logic, includes the swapped flag optimisation for early exit on already-sorted data, and notes best/worst case complexity (O(n) to O(n²)).

