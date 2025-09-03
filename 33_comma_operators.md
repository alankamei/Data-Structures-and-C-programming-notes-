## comma or , operators

1. Comma operator can be used as a "separator". 
e.g. int a = 3, b = 4, c = 8;  [ simply means multiple definitions]




2. Comma operator can be used as an "operator".
 e.g. int a = (3, 4, 8);  Output is 8;
  - Comma operator returns the rightmost operand in the expression and it simply evaluates the rest of the operatnds
  and finally reject them.

  ## Comma operator returns the rightmost operand in the expression and it SIMPLY EVALUATES THE REST OF THE OOPERANDS 
  and finally reject them.

  .e.g. 
  int var = (printf("%s\n", "HELLO!"), 5);
  printf("%d", var);

  -- 5 gets return but printf("%s\n", "HELLO!") will be evaluated first so
  -- Output: HELLO!
                5

3. Comma operator is having least precedence among all the operators available in C language.

e.g. 1
int a;
a = 3,4,8;

printf("%d", a);

-- here = have higher precedence than , it will treat like this  a = 3, 4, 8; [ remember 4 and 8 should be return to a variable but we don't have a variable here]

## e.g. 2
int a = 3, 4, 8;   [ this equivalent is int a = 3, int 4, int 8; which is invalid]
printf("%d", a);

NOTE: Comma operators acts like a separator within function calls and definitions, variable declarations and enum declarations.

OUTPUT: error



## e.g. 3

int a;
a = (3, 4, 8);

printf("%d", a);

NOTE: Bracket has the highest precedence than any other operator.


OUTPUT: 8 




## What is the output of the following c program fragment?

#include <stdio.h>

int main() {
    int var;
    int num;

    num = (var = 15, var+35);
    printf("%d", num);
    return 0;
}

OUTPUT: 50  

-- Do you know how I got this?