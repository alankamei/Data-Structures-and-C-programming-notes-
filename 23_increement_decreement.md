##

- Increment operator is used to increment the value of a variable by one. Similarly, decrement operator of a variable by one. Similarly, decrement operator is used to decrement the value of a variable by one.



- both increment and decrement are unary operators



## Increment and decrement operators

1. Pre-increment: ++a;    [ increment first then assign it to another variable]
2. Post-increement: a++; [ take the value first then increment the value]
3. Pre-decrement: --a; [ decrement first then take the value]
4. Post-decrement: a--; [ take the value first then decrement the value]



## You cannot use rvalue before or after increment/decrement operator.
e.g. (a+b)++; or ++(a+b); 
this gives lvalue errror


## lvalue(left value): simply means an object that has an identifiable location in memory (i.e. having an address).
- In any assignment statement "lvalue" must have the capability to hold the data
- lvalue must be a variable because they have the capability to store the data.
- lvalue cannot be a function, expression ( like a+b) or a constant like 3,4,etc


## rvalue: simply means an object that has no identifiable location in memory


lvalue = has a box (can store something) → can appear on left side of =

rvalue = just a value (no box) → can only appear on right side of =