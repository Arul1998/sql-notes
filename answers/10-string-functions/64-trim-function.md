# Lesson 64 Answer: TRIM Function

## Exercise

Display `CustomerName` and `CleanName`.

Use `TRIM` to remove spaces from the beginning and end of `CustomerName`.

## Sample Table

| CustomerId | CustomerName | City |
|---:|---|---|
| 1 |   Sarah   | London |
| 2 |  David | NULL |
| 3 | Priya  | Chennai |

## Answer

```sql
SELECT CustomerName,
       TRIM(CustomerName) AS CleanName
FROM Customers;
```

## Expected Result

### Result

| CustomerName | CleanName |
|---|---|
|   Sarah   | Sarah |
|  David | David |
| Priya  | Priya |
