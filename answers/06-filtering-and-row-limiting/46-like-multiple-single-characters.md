# Lesson 46 Answer: LIKE: Multiple Single-Character Wildcards

## Exercise

Display customers whose name has two characters followed by `ya`.

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
WHERE CustomerName LIKE '__ya';
```

## Expected Result

### Result

| CustomerId | CustomerName | City |
|---:|---|---|
| 2 | Priya | Manchester |
| 5 | Maya | Manchester |