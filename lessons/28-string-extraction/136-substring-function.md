# Lesson 136: SUBSTRING

`SUBSTRING()` extracts a specified number of characters starting at a chosen position. SQL Server character positions start at 1.

## Sample Table

| ProductId | ProductName | ProductCode |
|---:|---|---|
| 1 | Laptop | PRD-LAP-1001 |
| 2 | Mouse | PRD-MOU-2002 |
| 3 | Keyboard | PRD-KEY-3003 |
| 4 | Monitor | PRD-MON-4004 |

## Syntax

```sql
SUBSTRING(text, start_position, length)
```

## Example

```sql
SELECT SUBSTRING('EMP12345', 4, 3) AS Result;
```

## Exercise

Using `Products`, display `ProductId`, `ProductName`, and `CategoryCode`. Use `SUBSTRING()` to extract the three-letter category code at position 5 in each `ProductCode`.
