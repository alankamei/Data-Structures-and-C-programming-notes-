## let's understand through the example

main.c

#include <stdio.h>
#include <stdlib.h>

int main() {
    int value; 
    value = increement();
    value = increement();
    value = increement();

    printf("%d", value);
    return 0;
}



somefile.c ...

static int count;     [ this count is not visible to main.c anymore if we use static even if the count is global, it also retain it's value even if it's local/global]
int increement() {
    count =  count + 1;
    return count;
}

- you can only assign a constant literal ( or value ) to a static variable. ( you can't assign variable to static variable as its value)