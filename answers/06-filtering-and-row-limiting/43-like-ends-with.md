# Lesson 43 Answer: LIKE: Ends With

## Exercise

Display customers whose name ends with `n`.

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
WHERE CustomerName LIKE '%n';
```

## Expected Result

### Result

| CustomerId | CustomerName | City |
|---:|---|---|
| 3 | John | London |