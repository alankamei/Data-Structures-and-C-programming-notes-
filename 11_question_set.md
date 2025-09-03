## What is the output of the following c program fragment: 
#include <stdio.h>
int main(){
    printf("%d", printf("%s", "Hello World!"));
}
OUTPUT: Hello world!12

: printf not only prints the content of the screen. It also returns the number of characters that it successfully prints on the screen.


## What is the output of the following c program fragment?

int main() {
    printf("%10s", "Hello");
    return 0;
}

10 means that we need to print 10 characters and since we have only 5, the remaining 5 are used for white space .....Hello


## What is the output of the following c program fragment?

int main() {
    char c = 255;
    c = c + 10;
    printf("%d", c);
    return 0; 
}

: char hold 1 bytes only
: 265 exceeded 255 so we need to work this with binary, represents it and we get 9 
: simply 2^n mod where n is the bits [ C follows this modulo division if the range is exceeded]


## What does the following program fragment prints?

int main() {
    unsigned i = 1;
    int j = -4;
    printf("%u", i + j);
    return 0;
}

Ouput: Integer value depends from machine to machine [ but to get this perform 2's complement, also if %d we will get -3]