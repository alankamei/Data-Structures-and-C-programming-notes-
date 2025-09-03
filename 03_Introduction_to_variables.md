## Introduction to variables

- Glass and water

# Variables are names that refer to memory locations where data is stored.
! Declare variable before you use [ announcing the proerties of variable to the compiler] 
- properties: 1. Size of the variable 2. Name of the variable.

# Defining or Definition: allocating memoryt to a variable
- most of the time declaration and definition will be done at the same time but it also depends on the modifiers we used with a variable.


# e.g.
- int var;  [ int is a Data type: how much space a variable is going to occupy in the memory, var is a variable name]

# Initialization is when you assigned a value by the time you declared a variable e.g. int var = 10;

## We can change the value of a variable until you assigned constant. But multiple declaration of the same variable is not allow.

#include <stdio.h>

int main(){
    int var = 7;
    var = 4;
    printf("%d", var);
    return 0;
}

# you can also assigned another variable to a variable. [ var1 = var2 = var3 = 4;]