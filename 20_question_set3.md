1. What is the output of the following c program fragment?

#include <stdio.h>
int main() {
    int var = 0x43FF;

    printf("%x", var);
    return 0;
}

: here if we put 0x it is treated as hexadecimal values, it will print 43ff and 43FF for %X 



## Memory layout of C program:
                 ----> Command line arguments and environment variables
        STACK
          
        HEAP

        Uninitialized data (bss)    ------> Block started by symbol [ Uninitialized global, static (both local and global), constant global variables]

        Initialized data            -------> Read only and Read write   [ Global, extern, static ( both local and global), const global variables]

        Text/Code segment           ----->   [ Contains machine code of the compiled program]


## you can check the size of your c program using size yourexecutable.exe


here's the question.. [ check the scope of the variable also]

#include <stdio.h>
static int i;
static int i = 27;
static int i;

int main() {
    static int i;
    printf("%d", i);
    return 0;
}


this will print 0.
