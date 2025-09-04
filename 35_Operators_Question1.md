## What is the output of the following c program fragment? Assume size of integer is 4 bytes.

#include <stdio.h>
int main() {
    int i = 5;
    int var = sizeof(i++);
    printf("%d %d", i, var);

    return 0;
}


OUTPUT: 5 4 [ do you know why?]


NOTE:
- According to C99 standard:
    The sizeof operator yields the size (in bytes) of its operand, which may be an expression or a parenthesized name of a type. The size is determined from the type of the operand. If the type of the operand is a variable length array type, then the operand is evaluated; otherwise, the operand is not evaluated and the result is an integer constant.


