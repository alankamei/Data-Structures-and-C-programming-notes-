## Left shift operator

First operand  [ whose bits get left shifted] << Second operant [ Decides the number of places to shift the bits]

## Important points
- When bits are shifted left then trailing positions are filled with zeros.

e.g.

#include <stdio.h>

int main() {
    char var = 3;
    printf("%d", var<<1);
    return 0;
}

output is 6

- Left shift is equivalent to multiplication by 2^(rightOperant)  e.g. 3 x 2^(1) = 6