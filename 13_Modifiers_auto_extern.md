## Modifiers- auto and extern


- Auto means Automatic: Variables declared inside a scope by default are automatic variables.

Syntax: auto int some_variable_name;
Benefits: It won't waste memory, it get destroyed after used automatically.

NOTE: IF you won't initialize auto variable, by default it will be initialized with some garbage(random) value.
    : On the other hand, global variable by default initialized to 0.



## Extern Modifier

- int var;  [ Declaration and Definition, asking the compiler to allocate the memory to this var of integer datatype]
- extern int var; [ this is only declaration, this tells compiler not to allocate memory]
    : Extern is short name for external.
    : Used when a particular file needs to access a variable from another file.