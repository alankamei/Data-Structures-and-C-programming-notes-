## Defining scope of a variable:
# Local and Global variable


Scope = Lifetime

# The area under which a variable is applicable or alive.

# Strict Definition:  a block or a region where a variable is declared, defined and used and when a block or a region ends variable is automatically destroyed.

.e.g. 
#include <stdio.h>
 int main() {
    int var = 34;
    printf("%d", var);
    return 0;
 }

 int fun() {
    printf("%d", var);
 }


 ## Basic principle of scoping

 {

    Contents of outer block upto this point are visible to the internal block
    {

        contents of internal block are not visible to outer block

    }
 }

## example
 #include<stdio.h>
 int fun();

 int var = 10;  [ this is a Global variable]
 int main() {
    int var = 3;       [ this is a local variable]
    printf("%d\n", var);
    fun();
    return 0;
 }

 int fun() {
    printf("%d", var);
 }

 Can you check the output?
