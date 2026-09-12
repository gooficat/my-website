# A WORK IN PROGRESS

Everything in the top level scope in C is a declaration. It declares a symbol of some kind. The options are:

A variable. This is data. It can be static or not static. If it is static then it is not visible to other files.

```c
int this_var_holds_a_whole_number;
char this_is_a_character;
float i_am_a_decimal;

unsigned int i_cant_be_negative;

int *i_hold_a_memory_address_of_an_int;

struct {
	int a_child;
	struct {
		char foo;
	} a_struct_inside_another;
} I_am_multiple_vars_together;

char i_am_lots_of_vars_of_same_type_together[5040];


```

A function. This is a block of code. It can take in values and output values, even if those values are nothing.


This function takes in an int and returns another int;
```c
int my_func_returns_int_wow(int a_parameter) {
	return a_parameter + 123;
}
```


An external reference. This is a variable or function somewhere outside this file.

```c
extern int my_var;
int my_func(int c);
```

A typedef. This gives an alias to a specific type.
```c
typedef int ** foobar;
```



