# Expressions
Haumea has a rich set of operators which are summarized in the following table, along with their precedence. This is similar to the typical BIDMAS/PEDMAS system:

Precedence | Operators
--- | ---
0 | Literal numbers, variables, `( ... )`
1 | - (Negation)
2 | * (Multiplication), / (Division)
3 | + (Addition), - (Subtraction)
4 | > (Greater than), < (Less than), >= (Greater than or equal), <= (Less than or equal), = (Equals)
5 | and (Logical AND), or (Logical OR)

Precedence 0 is the highest, and 5 is the lowest. E.g, `5 * 2 + 3 >= 6 - 5 or 4 = 6` is parsed as
```
         (or)
        /   \_____
      (>=)        \
      /  \_        \
    (*)    \      (=)
    / \    (-)    / \
  (+)  5   / \   4   6
  / \     6   5
 2   3
```
