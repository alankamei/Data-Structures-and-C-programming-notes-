

## Fundamental Data Types (part-1) - Integer
- Integer can take upto 2 bytes or 4 bytes of memory space depending on the machine.
- 1 bytes = 8 bits, 4 bytes = 32 bits
- programmatically we use sizeof unary operator to check the size of a datatype  [ not a function]
- printf("%d", sizeof(int));



#               Range               #
- upper and lower limit of some set of data [ e.g. { 0,1,2,3,4}], then range is 0 to 4



## To understand the range of an integer we have to understand Decimal no. system first .i.e. 0 - 9
- Decimal number system: A human understandable number system. Also called as base 10 number system.
- Range: 0 - 9
- to represent 5 6 8 as a bigger digits 568 we must multiply each digit with each place value starting from rightmost with 10^0 x 8 + 10^1 x 6 + 10^2 x 5 where we get 568.

so like that it works for binary no. system but with 2^0, 2^1 and so on...

# Binary no. system: Machine Understandable number system. Also called aas base 2 no. system.
- multiply the binary digits with their place value and add them up to get the value
- e.g. 1 1 0 0  is 12

## Formula to calculate the range of integers we have
- 2^n - 1   where n is the no. of bits.
- but signed range are usually represented using 2's complement with the formula -2^n to +2^n-1   -1

## How you perform 2's complement?
- First convert it into binary, second convert it into 1's complement .i.e. turn all zeros into ones and ones into zeros, third add 1 to the 1's complement.

