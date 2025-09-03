## AS the name suggests - something that never change --> Constant

Once defined cannot be modified later in the code.

- We can define constant using #DEFINE and using the keyword const

#define Name Value [ #define PI 3.14159]    don't add semicolon at the end.

## Writing multiple lines using \

#define greater(x,y) if(x>y) \
            printf("%d is greater than %d", x, y); \
            else \
            printf("%d is lesses than %d", x, y);

int main() {
    greater(5,6);
    return 0;
}



## Some predefined macros like __DATE__, __TIME__ can print current date and time.


#include <stdio.h>

int main() {
    printf("DATE: %s\n", __DATE__);
    printf("TIME: %s\n", __TIME__);
    return 0;
}
