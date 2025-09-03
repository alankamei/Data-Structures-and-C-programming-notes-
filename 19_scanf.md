# What is scanf?
- Stands for Scan Formatted string

Accept character, string and numeric data from the user using standard input - keyboard.

e.e.g Accepting input and assigning the value into a variable

int var;
scanf("%d", &var);

## But why &?
While scanning the input, scanf needs to store that input data somewhere.
To store this input data, scanf needs to know the memory location of a variable.

And here the ampersand [ address of operator] comes to rescue.

&var means address of var not the content