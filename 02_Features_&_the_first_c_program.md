


## More features and a basic C code.

# Fetures of C
- Procdural programming: dividing the gigantic programs into much smaller programs called procedures or functions.
- Middle level language: C is a middle level language and it can perform
    * Direct access to memory through pointers.
    * Bit manipulation using bitwise operators.
    * Writing assembly code within C code.
- Popular choice for system levels apps.
- Wide variety of built in functions, standard libraries and header files like [ stdio.h, math.h, string.h, stdlib.h, isdigit, sqrt, time.h, ctype.h, malloc, etc..]


# High level vs Low level
- Both points to degree of abstraction:
    - High degree of abstraction means less effort. [ COBOL, FORTRAN, C++, Pascal,..]
    - Lower degree of abstraction means more efforts.  [ Assembly Language]

## How C codes looks like?
// This program will print the output Hi Alan on the console window

#include <stdio.h>  
int main()
{
    printf("Hi Alan);
    return 0;
}

- #include <stdio.h> is a preprocessor directive. It tells the preprocessor to include the contents of the standard header file stdio.h, which contains declarations of [ prototypes] input/output functions (like printf and scanf)

- Output of preprocessing is expanded source code [ Source Code --- Processor-->  Expanded Source Code --- Compiler ---> Machine Code ]
- main () is predefined you cannot change it.
- int main() [ this is a function annd also the entry point where the program starts]
- int here means that the function after completing all the execution it will return an integer value
- and return 0 indicates if the program completed successfully it will returns 0 and else other than 0.


## Syntax of a function
- Return_type name_of_the_function ( parameter_type name_of_parameter, , , ) {
    Set of statements
}

- printf() is a function but we don't add curly bracket but instead with ;, this is because its a predefined function somewhere in  c standard library so we just call them.


## Why Different files?
1. Header files [ like stdio.h] : It have declaration of functions. It tells your compiler which functions you will use in your program. and the preprocessor simply compiles those declaration with your actual source code and produce expanded source code.


 --- Now we have a program called Linker which actually maps down the prototypes mention by the preprocessor with the actual code which is in the C standard library [ it does not copy paste but simply maps]

2. C standard library: It have the actual definitions of functions [ stores the acutual code].

## So if everything is done by a compiler it will be a lot of work and will slow down the compiler ## 







