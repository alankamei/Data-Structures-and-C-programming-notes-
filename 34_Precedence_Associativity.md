## Precedence and Associativity of operators


- Precedence of operatros come into picture when in an expression we need to decide which operator will be evaluated first. Operator with higher precedence will be evaluated
first.

- Associativity of operators come into picture when precedence of operators are same and we need to decide which operator will be evaluated first.
    # Associativity can be either
    1. Left to right
    2. Right to left



## Precedence and associativity table


- the topmost operators have the highest precedence among all.

    CATEGORY                                        Operators                                           Associativity
    Paranthesis/brackets                            () [] -> . ++ --                                    Left to right
    Unary                                           ! ~ ++ -- + - * & (type) sizeof                     Right to lefft
    Multiplicative                                  * / %                                               Left to right
    Additive                                        + -                                                 Left to right
    Bitwise Shift                                   << >>                                               Left to right
    Relational                                      < <= > >=                                           Left to right
    Equality                                        == !=                                               Left to right
    Bitwise AND                                     &                                                   Left to right
    Bitwise XOR                                     ^                                                   Left to right 
    Bitwise OR                                      |                                                   Left to right
    Logical AND                                     &&                                                  Left to right
    Logical OR                                      ||                                                  Left to right
    Conditional                                     ? :                                                 Right to left
    Assignment                                      = += -= /= %= &= ^= |= <<=  >>=                     Right to left
    Comma                                           ,                                                   Left to right






## () - paranthesis in function calls
.e.g. int var = fun();


NOTE: = operator is having less precedence as compared to () therefor, () belongs to fun and fun will be treated as a function
And it looks like this:
int var = (fun());

## Member access operators ( -<  .)
- They are used to access members of structures [We will talk about structures later in this course.]
- Precedence of Postfix Increment/Decrement operator is greater than prefix increment/decrement
- Associativity of Postfix is also different from Prefix. Associativity of postfix operators is from left to right and that of prefix operators is from right to left.


## Important facts:

- Associativity can only help if there are two or more operators of same precedence and not when there is just one operator.
.e.g. 
int main() {
    int a; 
    a = fun1() + fun2();
    printf("%d", a);
    return 0;
}

int fun1() {
    printf("Alan");
    return 1;
}
int fun2() {
    printf("Kamei");
    return 1;
}

Which function is called first?
    - It is not defined whether fun1() will be called first or wheter fun2() will be called. Behaviour is undefined and output is compiler dependent.


- Operators with same precedence have same associativity as well.

# What is the output of the following C program fragment?
- #include <stdio.h>
int main() {
    int a = 10, b = 20, c = 30, d = 40;

    if (a <= b ==  d > c) {
        printf("TRUE");
    }
    else {
        printf("FALSE");
    }
    return 0;
}

-- OUTPUT: TRUE. [ do you know why?]