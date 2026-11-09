# Lesson 147: NCHAR

`NCHAR()` converts a Unicode numeric value to a Unicode character. It can produce characters from international scripts such as Tamil.

## Sample Table

| ProductId | ProductName | UnicodeCode |
|---:|---|---:|
| 1 | Laptop | 65 |
| 2 | Mouse | 66 |
| 3 | Keyboard | 67 |
| 4 | Monitor | 2980 |

## Syntax

```sql
NCHAR(unicode_number)
```

## Example

```sql
SELECT NCHAR(2980) AS TamilCharacter;
```

## Exercise

Using `Products`, display `ProductId`, `ProductName`, and `UnicodeCharacter`. Convert each `UnicodeCode` into its corresponding character using `NCHAR()`.
