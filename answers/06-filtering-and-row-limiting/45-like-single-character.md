# Lesson 45 Answer: LIKE: Single-Character Wildcard

## Exercise

Display customers whose name has any first character followed by `ohn`.

## Sample Table

| CustomerId | CustomerName | City |
|---:|---|---|
| 1 | Arul | London |
| 2 | Priya | Manchester |
| 3 | John | London |
| 4 | Sara | Birmingham |
| 5 | Maya | Manchester |

## Answer

```sql
SELECT *
FROM Customers
WHERE CustomerName LIKE '_ohn';
```

## Expected Result

### Result

| CustomerId | CustomerName | City |
|---:|---|---|
| 3 | John | London |