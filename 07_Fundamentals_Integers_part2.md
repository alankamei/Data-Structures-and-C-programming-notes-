## OUtline
1. Modifiers ( short,long, signed, unsigned) used for integer.
2. Some programming examples.

Long [ 8 bytes] and Short [decide less or more]
-- sizeof(short) < = sizeof(int) <=  sizeof(long)

### Range of integer

2 Bytes [ 16 bits]
: Unsgined range: 0 to 65535 [ by applying: 2^n - 1 where n is the no of bits]
: signed range: -32768 to +32767

4 Bytes [ 32 bits]
: Unsigned range: 0 to 4294967295 [ by applying: 2^n - 1]
: signed range: -2147483648 to +2147483648 [ by applying: -2^(n-1) to +2^(n-1) -1]

NOTE:
1. We use 2's complement to represent negative integers.
2. By default int some_variable_name; is signed integer variable.
3. Unsigned int some_variable_name: allows only positive values.




## program to print the signed range. [ 4 bytes]

#include <stdio.h>
#include <limits.h>

int main() {
    int var1 = INT_MIN;    [ INT_MIN is a symbolic constant]
    int var2 = INT_MAX;

    printf("range of signed integer is from: %d to %d", var1, var2);
    return 0;
}

# for unsgined range use:
1. unsigned int var1 = 0;
2. unsigned int var2 = UINT_MAX;
3. use %u as a format specifier.

# for short range
1. short unsigned int var1 = SHRT_MIN; [ the order of short unsigned and unsigned short doesn't matter]
2. SHRT_MAX;
3. %d

# for unsigned short
1. 0
2. USHRT_MAX;
3. %u

# long unsgined
1. %lu

# long integer
1. %ld

# long long integer
1. %lld

# unsgined long long
1. %llu



NOTE:
if sizeof(long int) = 4 bytes
then sizeof(long long int) = 8 bytes

else

if sizeof(long int) = 8 bytes
then sizeof(long long int ) = 8 bytes