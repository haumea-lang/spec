# Functions
## Definitions
You can declare a function with the `to` keyword like so:
```
to <name> [with (<param-1>, ... <param-n>) <statement>
```
where `<name>` is just any identifier (A string that matches the RE /a-zA-Z_/), <param-n> is also an identifier that is a parameter to the function, and <statement> is the statement that is run when the function is executed. The parameter list (`with (<param-1>, ... <param-n>)`) is optional, and if it is omitted the function is assumed to take zero parameters. Some example function definitions:
```
to add_one with (n) return n + 1

to foo do
    display(1)
    display(2)
    display(3)
end
```
You can return a value from the function by using the `return` statement, e.g `return n * 2`

The function named "main" is special, as it is run when the program starts.

## Calling
A function is called by writing its name followed by the parameters passed to the function inside parenthesis. E.g `foo(1, 2)` or `bar()`
They can be called as both a statement and as part of an expression, e.g you can do both `foo()` stand alone and `foo() + 1`.
