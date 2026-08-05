# Lesson 44: LIKE: Contains

Place `%` on both sides of text to find values containing that text anywhere.

## Sample Table

| CustomerId | CustomerName | City |
|---:|---|---|
| 1 | Arul | London |
| 2 | Priya | Manchester |
| 3 | John | London |
| 4 | Sara | Birmingham |
| 5 | Maya | Manchester |

## Syntax

```sql
SELECT columns
FROM table_name
WHERE column_name LIKE '%text%';
```

## Example

```sql
SELECT *
FROM Customers
WHERE CustomerName LIKE '%ar%';
```

The matching text can appear at the beginning, middle, or end.

## Exercise

Display customers whose name contains `ri`.