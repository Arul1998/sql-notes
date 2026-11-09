# Lesson 145: CHAR

`CHAR()` converts a numeric character code into a character. It is the reverse of `ASCII()` for standard ASCII values.

## Sample Table

| ProductId | ProductName | CategoryCode |
|---:|---|---:|
| 1 | Laptop | 69 |
| 2 | Mouse | 77 |
| 3 | Keyboard | 75 |
| 4 | Monitor | 83 |

## Syntax

```sql
CHAR(ascii_number)
```

## Example

```sql
SELECT CHAR(66) AS Result;
```

## Exercise

Using `Products`, display `ProductId`, `ProductName`, and `CategoryLetter`. Convert the numeric `CategoryCode` values into characters using `CHAR()`.
