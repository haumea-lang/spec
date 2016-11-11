# Loops
Haumea has 3 different kinds of loops.

## Forever loops
Forever loops just loop forever. For example:
```
forever do
  display(1)
  display(2)
end
```
will print 1 and 2 to your terminal forever (or until you stop it)

## While loops
While loops will loop while the condition is true. For example:
```
while foo() bar()
```
Will keep calling bar() as long as foo() returns a truthy value (any number other than 0, but normally 1)

## For each loops
A for each loop loops over a range of numbers, assigning a variable to each number in turn. For example:
```
for each x in 0 to 10 by 2 do
  display(x)
end
```
The **by** clause is optional, so can also write a for each loop like the following:
```
for each y in 1 to 5 do
  display(y)
end
```
The range of numbers looped over is _inclusive_ on the lower bound (the first number), but _exclusive_ on the upper bound (the second number). E.g, the code fragment above would display
```
1
2
3
4
```
NOT
```
1
2
3
4
5
```
If you want that second result (inclusive), you may use **through** rather than **to**:
```
for each z in 1 through 5 do
  display(z)
end
```
This will result in 1 to 5, _including_ 5 itself!
