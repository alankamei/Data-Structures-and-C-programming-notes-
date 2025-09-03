1. What is the output of the following c program fragment?

#include <stdio.h>

int main() {
    int a = 4, b = 3;
    printf("%d", a+++b);
    return 0 ;
}


# to understand the weird a+++b we must understand one concept called TOKEN generation.

- Lexical analysis is the first phase in the compilation process.  [ finding out the meaning/information behind it]
- Lexical analyzer (scanner) scans the whole source program and when it finds the meaningful sequence of characters (lexemes)
then it converts it into a token.

- Token: lexemes mapped into token-name and attribute-value.

.e.g. int --->  <keyword, int>   

- It always matches the longest character sequence.
e.g. int a = 5; 

there the lexical analyzer will scan them one by one and converts it to token

tokens: int   a  = 5   ;    [ here 5; are together but they're not a meaningful sequence so they are generated with different 2 tokens]

### Now a++b

token:   a    ++   +   b  [ we got 4 tokens]

a+++b will give 7



### now for a + ++ b

now we get a+ ++b [ this will give 8]