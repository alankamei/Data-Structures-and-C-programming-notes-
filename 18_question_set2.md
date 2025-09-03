1. What is the output of the following c program?

int main() {
    int  var = 052;
    printf("%d", var);
    return 0;
}

: When we place any 0 in the value it is treated as octal and not decimal.

Internally?  it converts 052 into octal. use place value of octal .i.e. 8^0 .....

we get 5 * 8 + 2 * 1 = 42. so 42 gets printed.


::: ### if we use %o [ octal] we will get 52

2. What is the output of the following c program?

#include <stdio.h>
#define STRING "%s\n"
#define NESO "Welcome to Neso Academy!"

int main() {
    printf(STRING, NESO);
    return 0;
}

