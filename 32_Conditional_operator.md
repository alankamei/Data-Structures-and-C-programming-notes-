## Conditional Operators

- Syntax:        ? :

- It is a ternary operator. [ it requires three operands]

# why do we need this conditional operator? Let's check out

char result;
int marks;
if( marks > 33)
    {
        result = 'p';
    }
else
    {
        result = 'f';
    }


## Alternate code with conditional operator but shorter

char result;
int marks;
result = (marks > 33) ? 'p' : 'f';


---- things to uderstand from there ----

- ( marks > 33 ) is a boolean expression, therefore it will return either TRUE or FALSE.

- so if the condition ( marks > 33) is TRUE it will store 'p' in the variable result otherwise 'f'.
- ( marks > 33 ) ? 'p' : 'f' is a conditional expression, which is after all an expression, therefore it is an r-value and result is -lvalue.



### Quick facts checklist

- Conditional operator is the only ternary operator available in the list of operators in C language.
- As in Expression1 ? Expression2: Expression3, expression1 is the boolean expression. If we simply write 0 instead of some boolean expression
    then that simply means FALSE and therefore expression3 will be evaluated.
    e.g. int result;
    result = 0 ? 2 : 1



    ## What is the output of the following c program

    #include <stdio.h>
    int main() {
        int var = 75;
        int var2 = 56;
        int num;

        num = sizeof(var)? (var2 > 23 ? ((var== 75) ? 'A' : 0) : 0) : 0;

        printf("%d" num);
        return 0;
    }


    --------   In C, a character constant like 'A' is not stored as the letter itself but as its ASCII code value.

The ASCII value of 'A' is 65.

Since num = 'A'; assigns the ASCII value, when we print it using %d, it displays 65 instead of the character.

 If we had used %c, then it would print the character A directly.