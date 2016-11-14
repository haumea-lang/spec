# Functions

## Declare
You can declare a function with the **to** keyword like so:

```
to <name> [with (<variable>, <variable>, <variable>...) [as <type>] <statement>
```

Where:
- `<name>` is just any identifier (a word with only uppercase/lowercase characters and `_`)
- `<variable>`s are also identifiers that are taken as parameters.
- `<statement>` is the statement that is run when the function is executed.
- The **parameter list** (`with (<variable>, <variable>, <variable>)`) is optional, and if it is omitted the function is assumed to take zero parameters.
- The **return type** (`as <type>`) is a [type](variables-and-types.md#types). If ommitted, the function must [not return anything](variables-and-types.md#none).

Some examples:
```
to add_one with (integer n) as integer return n + 1

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
