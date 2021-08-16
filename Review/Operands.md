# Operands
[Oracle documentation](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/opsummary.html)
[Precedence Table](http://www.cs.bilkent.edu.tr/~guvenir/courses/CS101/op_precedence.html) 
 - => Also known as order of operations, higher numbers have higher precedence

| Operand | Description |
|---|---|
| + | Add |
| - | Subtract |
| / | Divide |
| * | Multiply |
| % | Modulus/Remainder operator |
| == | Literal equal operator returns a true or false value |
| != | Not equal operator returns a true or false value |
| > | Greater than operator returns true or false value |
| < | Less than operator returns true or false value |
| <= |Less than or equal to operator |
| >= | Greater than or equal to operator|
| && | Logical AND operator, checks if both conditions are true. -> Note: Operates on boolean operands, checking if a condition is true or false |
| \|\| | - Logical OR operator, checks if any of the conditions are true -> Note: Operates on boolean operands, checking if a condition is true or false |
| & | Bitwise AND operator, works at the bit level, takes the bits of the results and preforms an AND operation on them |
| \| | Bitwise OR operator, works at the bit level, takes the bits of the results and preforms an OR operation on them |
| ~ | Bitwise compliment, unary operator, returns the one's compliment representation of the input value -> Note: The compiler will return the 2's complement of that number |

### Ternary Operator
```java 
// Ternary Operator
// The ternary operator is a shorthand for an if else statment when assigning a
// variable, however unlike in javascript, in java it can only be used when
// assigning a variable.
// Examples:
int val = condition ? expression1 : expression2;
String huh = boonleanValue ? huhValueIfTrue : huhValueIfFalse;
```

## Abbreviations
| Abbreviation | Equivalent |
|---|---|
| `x++` | `x = x + 1;`|
| `x--` | `x = x - 1;`|
|`x += y `|` x = x + y;`|
| `x *= y `|` x = x * y;`|
|`x /= y `|` x = x / y;`|
|`x -= y` |` x = x - y`|