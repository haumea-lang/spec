# Variables
Haumea does not currently have global variables, only function local variables. This means that any variable declared inside a function may only be accessed within it.

At the moment, **all variables are integers**, aka whole numbers.

You can declare a variable using the **variable** statement like so:
```
variable x
variable foo
```
You can only declare one variable per variable statement.

You can use the value of the variable by just using the variable's name.

You can set the value of a variable by using the `set ... to ...` statement:
```
set x to 5
set foo to x
```

You can also change the value of a variable by using the `change ... by ...` statement:
```
change x by 1
change foo by -9
```
`change x by y` is exactly the same as `x += y` in C-like languages.
