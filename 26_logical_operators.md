## C have &&, ||, !


&& returns true if only all the condiditons are true.

|| returns true if one condition is true

! operator is used to complement the condition under consideration.

## Concepts of short circuit in logical operators
- Short circuit in case of &&: simply means if there is condition anywhere int he expression that returns false, then the rest of the conditions after that will not be evaluated.

#include <stdio.h>

int main() {
    int a = 5, b = 3;

    int incr;

    incr = (a<b,) && (b++);
    printf("%d\n", incr);

    printf("%d", b);

    return 0;


}


## Since the first condition is false it won't evaluate further, and it will print 0 and 3 [ false prints 0 and true prints 1]


- b++ will be increment if the condition is true


### Short circuit in case of ||: simply means if there is a condition anywhere in the expression that returns True, then the rest of the conditions after that will not be evaluated.

.e.g. incr = ( a>b) || (b++)

here b++ is not evaluated since a>b is true, it simply prints the b value .i.e 3