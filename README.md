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


[PROJECT WORKS]   
1. Parcel Weight Charge Calculator-Using aimple while loop to provide reiteration, and using simple loop to differentiate boundaries.Function allows the addition of additional vlaues needed.
<img width="629" height="381" alt="image" src="https://github.com/user-attachments/assets/4db2f382-3245-4810-914a-b3cf823ecf2a" />
Figure 1 shows the ability for users to enter their input.Entering “1” will allow user to enter their weight.
<img width="561" height="609" alt="image" src="https://github.com/user-attachments/assets/cf53c87e-e6ac-4883-a84b-a2735ee4b415" />
Figure 2  shows the programme’s ability to not only take different user’s input, but accurately calculate based on their weight charges to their appropriate weight boundaries.
<img width="628" height="279" alt="image" src="https://github.com/user-attachments/assets/947dafd5-17bf-4346-a168-2d2a4b6235cf" />
 Figure 3 shows the ability to reiterate until the user chooses to enter “0” to exit the programme.
<img width="497" height="277" alt="image" src="https://github.com/user-attachments/assets/e41ca426-97fe-4006-a9c3-6531c9ecbd00" />
In figure 4, there were possibilities where users could select a wrong option due to typo issues on the keyboard. The programme is able to re-prompt users to enter an option to continue.
<img width="575" height="399" alt="image" src="https://github.com/user-attachments/assets/7cc047ab-2fbf-4c95-b3e3-13b0e3f906bf" />
In figure 5, it shows the programme’s ability to detect out of boundary weight values, and are able to bring the user back to the menu in the events where they choose to exit the programme.


2. Property Stamp Duty Calculator-Design an algorithm that will prompt for and receive the purchase price of a property and property type (residential or non-residential) and calculate the buyer’s stamp duty and print
the value. Using a function to calculate different type of property type. Using While loop to provide re-iteration of programme.
<img width="675" height="286" alt="image" src="https://github.com/user-attachments/assets/364fe4c1-a444-4a91-bb18-712dc12dfa69" />
-Programme was able to process the user's option input and identify the correct Residential property type.
-It was also able to pass the property cost into the function to perform the appropriate calculation based on the type of property, and thereafter passing it back to the main function.
<img width="643" height="365" alt="image" src="https://github.com/user-attachments/assets/e0e62617-7cfb-4e94-bd2b-857c23b659bd" />
-The programme is able to reiterate and allow reuse for user.
-It is also able to identify the correct Property type to its appropriate Option(option 2).
-And passing the property cost to the function and computed the correct stamp duty
<img width="572" height="268" alt="image" src="https://github.com/user-attachments/assets/520558d6-131c-4b8c-869a-e7bfdd5427ba" />
Error handling of incorrect Option entered, will prompt user to re-enter a valid option.

3. Monthly Sales Tracker
<img width="500" height="495" alt="image" src="https://github.com/user-attachments/assets/1f2b6130-a3f5-49a9-b619-f3761b2eaace" />
-Ability of programme to ask for user’s sales input data for every month,and are able to give a report summary on the lowest sales, highest sales, the sum of all sales(Total Sales) and Average Sales.
<img width="573" height="693" alt="image" src="https://github.com/user-attachments/assets/29a35100-09f3-4e9c-bbbe-02d525bd940d" />
-Programme is able to process user’s choice to verify if record exist in the array. It is also able to bring user back to the menu for other choices soonafter.
<img width="511" height="593" alt="image" src="https://github.com/user-attachments/assets/211132bc-4295-42c1-9a00-02a9a0231daa" />
-Option L will allow user to access the selection sorted list of sales data in ascending format. This proves that the sales data was able to be passed into sorting function.
-Error Handling of incorrect Option entered, will prompt user that option is incorrect and given the option to re-enter again.







