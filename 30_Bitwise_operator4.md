## Bitwise ~ XOR operator 



## To understand this operator we must first understand what is 
- inclusive OR
- exclusive OR   [ XOR]

## Inclusive OR [ the other name of OR]

- Either A is 1 or B is 1 or Both are 1, then the output is 1.
- Including BOTH
- It is same as OR

e.e.g

        A               B               A OR B
        0               0                   0
        0               1                   1
        1               0                   1
        1               1                   1



## Exclusive OR
- Either A is 1 or B is 1 then the output is 1 but when both  A and B are 1 then output is 0.
- Excluding BOTH



e.e.g

        A               B               A OR B
        0               0                   0
        0               1                   1
        1               0                   1
        1               1                   0


### Bitwise XOR is binary operator. It takes two numbers and perform bitwise XOR.
### Result of XOR is 1 when two bits are different otherwise the result is 0.


## Example of XOR ^ to understand better

    7 ---> 0 1 1 1 
    4 ---> 0 1 0 0 
    3 ---> 0 0 1 1

    so 7 XOR 4 we get 3.  

code::::

What is the output of the following program snippet?

#include <stdio.h>

int main() {
    int a = 4, b = 3;
    a = a ^ b;
    b = a ^ b;
    a = a ^ b;

    printf("After XOR, a = %d and b = %d", a, b);
    return 0;
}






