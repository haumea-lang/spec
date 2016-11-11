# Blocks
To combine multiple statements itno one, Haumea provides the `do ... end` statement. It works like so:

```
do
  <statement-1>
  <statement-2>
  <statement-3>
  ...
  <statement-n>
end
```

The `do ... end` statement wraps around a group of statements and makes them one statement. This is mainly used for `if ... then ... else ...` and functions to allow multiple statements even though they only work with single statements, e.g.

```
variable wat
set wat to 0

if 1 = 2 change wat by 1
else do
  /* many things */
  display("Haumea is sane")
  display("Haumea is cool")
end
```
