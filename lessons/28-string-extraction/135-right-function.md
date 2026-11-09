# Lesson 135: RIGHT

`RIGHT()` extracts a specified number of characters from the end of a string.

## Sample Table

| ProductId | ProductName | ProductCode |
|---:|---|---|
| 1 | Laptop | LAP1001 |
| 2 | Mouse | MOU2002 |
| 3 | Keyboard | KEY3003 |
| 4 | Monitor | MON4004 |

## Syntax

```sql
RIGHT(text, number_of_characters)
```

## Example

```sql
SELECT RIGHT('EMP12345', 5) AS CodeNumber;
```

## Exercise

Using `Products`, display `ProductId`, `ProductName`, and `ProductNumber`. Use `RIGHT()` to extract the last four characters of each `ProductCode`.
