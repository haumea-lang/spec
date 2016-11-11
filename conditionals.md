# Conditionals
Haumea has just one statement for working with conditionals, the **if** statement. The if statement works like this:
```
if <cond> then <if-clause>
else <else-clause>
```
`<cond>` is an expression, and both `<if-clause>` and `<else-clause>` are statements. The **else** clause is optional.

For example:
```
if n = 1 then return 5
else do
  foo()
  return 0
end

if bar() then do
  baz()
  foo()
end
```
