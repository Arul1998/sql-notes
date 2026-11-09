# Lesson 144: ASCII

`ASCII()` returns the numeric character-code value of the first character of a string. For standard ASCII letters, `A` is 65.

## Sample Table

| ProductId | ProductName |
|---:|---|
| 1 | Laptop |
| 2 | Mouse |
| 3 | Keyboard |
| 4 | Monitor |

## Syntax

```sql
ASCII(text)
```

## Example

```sql
SELECT ASCII('Apple') AS FirstLetterASCII;
```

## Exercise

Using `Products`, display `ProductId`, `ProductName`, and `FirstLetterASCII`. Use `ASCII()` to find the numeric value of the first character of each `ProductName`.
