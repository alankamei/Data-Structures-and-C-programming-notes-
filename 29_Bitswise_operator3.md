## Right shift

First operant >> Second operand

## Immportant notes
- When bits are shifted right the leading positions are filled with zeros.


#include <stdio.h>

int main() {
    char var = 3;

    printf("%d", var>>1);

    return 0;
}

- Right shifting is equivalent to division by 2^(rightOperand) .i.e. 3/2^(1)