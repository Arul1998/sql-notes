# Lesson 134: LEFT

`LEFT()` extracts a specified number of characters from the beginning of a string.

## Sample Table

| ProductId | ProductName | ProductCode |
|---:|---|---|
| 1 | Laptop | LAP1001 |
| 2 | Mouse | MOU2002 |
| 3 | Keyboard | KEY3003 |
| 4 | Monitor | MON4004 |

## Syntax

```sql
LEFT(text, number_of_characters)
```

## Example

```sql
SELECT LEFT('EMP12345', 3) AS Prefix;
```

## Exercise

Using `Products`, display `ProductId`, `ProductName`, and `ProductPrefix`. Use `LEFT()` to extract the first three characters of each `ProductCode`.
