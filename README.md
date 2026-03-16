# C-Prog-MUS1
C Programme Practices and Assessment for my Bachelor's Module
Topics Demonstrated
1. Loops
Loops are used throughout the programs to iterate over data, process user input, and drive repetitive logic. All three major loop types are covered:

for loop — used when the number of iterations is known in advance (e.g., iterating over array indices).
while loop — used for condition-driven repetition (e.g., reading input until a sentinel value is entered).
do...while loop — used when the loop body must execute at least once (e.g., menu-driven programs).

Nested loops are also demonstrated where appropriate, such as when processing 2D arrays or generating patterns.

2. Dynamic Arrays
Dynamic memory allocation allows programs to manage memory at runtime rather than compile time. This section demonstrates:

Allocating memory on the heap using malloc() and calloc().
Resizing allocations using realloc() when the data size is unknown in advance.
Freeing memory with free() to prevent memory leaks.
Checking allocation success by verifying that returned pointers are not NULL.

Example use case: building a dynamically growing list of integers entered by the user.
cint *arr = malloc(capacity * sizeof(int));
if (arr == NULL) {
    fprintf(stderr, "Memory allocation failed\n");
    exit(EXIT_FAILURE);
}

3. Characters and Strings
This section covers character-level operations and string manipulation in C:

Using the char data type and understanding ASCII values.
Reading and writing individual characters with getchar() / putchar().
Working with character arrays (C strings) and the null terminator \0.
Using standard library functions from <string.h> such as strlen(), strcpy(), strcmp(), and strcat().
Classifying characters using <ctype.h> functions like isalpha(), isdigit(), and toupper().

Example use case: reversing a string in-place and converting it to uppercase.

4. Pointers and Addresses
Pointers are one of C's most powerful (and most challenging) features. This section demonstrates a solid understanding of:

Declaring and initialising pointers using the address-of operator &.
Dereferencing pointers with * to read and modify values.
Pointer arithmetic — advancing through arrays by incrementing pointer addresses.
The relationship between arrays and pointers.
Passing pointers to functions to enable pass-by-reference behaviour.
Double pointers (**) for modifying pointer variables inside functions.

cint value = 42;
int *ptr = &value;

printf("Value:   %d\n", value);
printf("Address: %p\n", (void *)ptr);
printf("Via ptr: %d\n", *ptr);

5. Functions
Functions are the building blocks of structured programming. This section demonstrates:

Declaring functions with appropriate return types and parameter lists.
Separating function declaration (prototype) from definition.
Passing arguments by value and by pointer (reference).
Returning values from functions, including returning pointers to heap-allocated data.
Recursive functions — functions that call themselves to solve problems like factorial calculation or binary search.

All functions follow a single-responsibility principle: each function does one thing and does it well.

6. Modularity
Good C programs are split across multiple files for maintainability and reuse. This project demonstrates modularity through:

Header files (.h) — contain function prototypes, constants (#define), and type definitions shared across files.
Source files (.c) — contain function implementations, each file grouped by logical responsibility.
Include guards — #ifndef / #define / #endif blocks in every header to prevent double inclusion.
main.c — serves as the entry point only; all logic is delegated to dedicated modules.

Project File Structure
assessment/
│
├── main.c              # Entry point — ties modules together
│
├── loops/
│   ├── loops.h         # Loop demonstration prototypes
│   └── loops.c         # Loop implementations
│
├── dynamic_array/
│   ├── dynamic_array.h # Dynamic array prototypes & structs
│   └── dynamic_array.c # malloc/realloc/free implementations
│
├── strings/
│   ├── strings.h       # Character & string function prototypes
│   └── strings.c       # String manipulation implementations
│
├── pointers/
│   ├── pointers.h      # Pointer demonstration prototypes
│   └── pointers.c      # Address, dereference, arithmetic demos
│
├── functions/
│   ├── functions.h     # Utility function prototypes
│   └── functions.c     # Recursive and utility function implementations
│
└── Makefile            # Build rules for compiling all modules

How to Compile and Run
Requirements

GCC (GNU Compiler Collection) or any C99-compatible compiler
Linux / macOS terminal, or Windows with MinGW / WSL

Compile all modules
bashmake
Or manually with GCC:
bashgcc -Wall -Wextra -std=c11 -o assessment \
    main.c \
    loops/loops.c \
    dynamic_array/dynamic_array.c \
    strings/strings.c \
    pointers/pointers.c \
    functions/functions.c
Run
bash./assessment
Clean build artefacts
bashmake clean

Key Concepts Summary
TopicConcepts ShownLoopsfor, while, do...while, nested loopsDynamic Arraysmalloc, calloc, realloc, free, NULL checksCharacterschar, ASCII, <string.h>, <ctype.h>, C stringsPointers&, *, arithmetic, double pointers, pass-by-referenceFunctionsPrototypes, scope, recursion, return valuesModularityHeader files, source separation, include guards, Makefile
