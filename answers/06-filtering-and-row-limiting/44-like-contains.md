# Lesson 44 Answer: LIKE: Contains

## Exercise

Display customers whose name contains `ri`.

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
WHERE CustomerName LIKE '%ri%';
```

## Expected Result

### Result

| CustomerId | CustomerName | City |
|---:|---|---|
| 2 | Priya | Manchester |