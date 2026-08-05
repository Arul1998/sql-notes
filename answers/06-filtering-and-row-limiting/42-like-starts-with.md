# Lesson 42 Answer: LIKE: Starts With

## Exercise

Display customers whose name starts with `M`.

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
WHERE CustomerName LIKE 'M%';
```

## Expected Result

### Result

| CustomerId | CustomerName | City |
|---:|---|---|
| 5 | Maya | Manchester |