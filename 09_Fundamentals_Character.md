## OUTLINE
- Brief  overview on character data type.
- Size of characters
- Range of characters
- Difference between signed and unsigned characters.

# size of char is 1 byte which is equal to 8 bits.

- A char can only hold one character with this format 'N', with a format specifier %c

# here
- char some_variable_name = 'N'
- char some_variable_name = 65

## Size and range of a character
- 1 Bytes = 8 bits
- Unsigned: 0 to 255
- Signed: -128 to +127

## Remember for every negative values we use 2's complement representation.

## code

char var = -128
printf("%c", var);
return 0;  [ try this out]