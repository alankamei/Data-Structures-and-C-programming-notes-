## Introduction to bitwise operators:

As name suggests - it does bitwise manipulation.

&, |, ~, <<, >>, ^

~ : NOT
<<: Left shift                         >>: Right shift
^: XOR


### Bitwise AND (&) operator

- It takes two bits at a time and perform AND operation.
- AND (&) is binary operator. It takes two numbers and perform bitwise AND.
- Result of AND is 1 when both bits are 1.


### Bitwise NOT (~) operator

- NOT is a unary operator.
- Its job is to complement each bit one by one.
- Result of NOT is 0 when bit is 1 and 1 when bit is 0.


------------------ Difference betweeen bitwise and logical operators ----------------------

#include <stdio.h>

int main() {
    char x = 1, y = 2;

    if( x&y)                                            [ 1 = 0000 0001 and 2= 0000 0010      performing bitwise & we get 0000 0000 which is 0, so it's false]
        printf("REsult of x&y is 1");
    if ( x&&y)                                                      [ TRUE && TRUE = 1]
        printf("Result of x&&y is 1");

    return 0;
}





