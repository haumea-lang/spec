# Variables
In Haumea, all variables must:
- Have a name comprised of uppercase characters, lowercase characters, and `_`
- Have a [type](#types)
- Never share a name with a keyword (`do`, `to`, `end`, `if`, etc)

You can use a variable simply by using its name:
```
display(my_variable)
```

## Declare
The **declaration statement** may be used to declare a variable's existence if you don't want to give it a value immediately; otherwise you may use the [set statement](#declare-and-assign) to declare it at the same time you give it a value. One can only declare **one variable per declaration statement**.
```
<type> <name>
```

Such as:
```
string foo
integer bar
float baz
```

## Assign
The **set ... to ... statement** may be used to assign a value to a variable:
```
set <name> to <value>
```

e.g.
```
set foo to "hello"
set bar to 25
set baz to 3.5
```

### Declare and Assign
It is possible to both declare _and_ assign a value to a variable in the same statement with the **set ... to ... statement**:

```
set string planet to "Earth"
```

Which declares a string called `planet` with the value `"Earth"`.

# Types

Haumea currently has three types;
|  identifier  | description  | example   |
| ------------ | ------------ | --------- |
| **string**   | Text         | `"Hello"` |
| **integer**  | Whole number | `172`     |
| **float**    | Decimal      | `1.0`     |

You cannot change the type of a variable.

## None
Note, there _is_ another type, `none`, which **cannot be assigned to a variable**. `none` is returned automatically by all [functions](functions.md) that do not have a [return type](functions.md#return-type).
