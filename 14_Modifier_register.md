## Modifier _ register


                    Register memory   [ fastest but very small memory]
                    Cache memory
                    Main Memory    [ primary memory]
                    Magnetic Disks      [ Auxillary memory]
                    Magnetic tapes


:::: What is register modifier?

- syntax: register some_data_type some_variable_name

#include <stdio.h>
int main() {
    register int var;
    return 0;
}


- Register keyword hints the compiler to store a variable in register memory.

