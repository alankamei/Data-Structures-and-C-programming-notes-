## Float, Double and Long double


They are used for representing a fractional numbers or real numberes:
for e.g. 3.14, 0.678, -3276.789, 0.00000009999


- Float follows IEEE 754 single precision floating point
- Doubel follows IEEE 754 double precision floating point
- Long double follows extended precision floating point

## Float follows IEEE 754 single precision floating point

Step 1. Convert given no. into binary no.

- e.g. 3066.25 
- 3066: 101111111010
- 0.25 x 2 = 0.5 so the carry is 0 [ see the integer part is zero so we need to further mulply 0.5 till we get 1 in the integer part]
- 0.5 x 2 = 1.0 and the carry is 1 [ so we stop]
- we took the carry bottom down .i.e. 0.25 is represented as 0.01
- 3066.25 is represented as 101111111010.01

Step 2. Represent binary no. into scientific notation
- to do this jump the . (point to the leftmost first digit .i.e. 1.0111111101001) and it took 11 digits to get there
-  so we can write 1.0111111101001 x 2^11

Step 3. IEEE 754 floating point single precision 32 bit
    .i.e 1 bit [ for signed +ve( represents with 0) and -ve( represents with 1)]   8 bits exponents [ exponent bias + power]   23 mantisa [ fill the rightmost with 0's if necessary]

    - then our first bit is 0, for 8 bits exponents the formula is 2^(k-1) + power .ie 2^(8-1) + 11 = 138 = 10001010, now mantissas are those after point.. 0111 1111 0100 1000 0000 000
    so this is how you represent floating point nos.

#### Float can represents fractional digits upto 7 digits precisely starting from the first place itself.

### Double can represent upto 16 %lf of %f
### long double can represent upto 19 digits  %Lf 