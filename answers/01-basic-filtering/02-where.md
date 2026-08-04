# Lesson 2 Answer: WHERE

## Exercise

Display `CustomerName` and `City` for customers who live in `Birmingham`.

## Sample Table

### Customers

| CustomerId | CustomerName | City |
|---:|---|---|
| 1 | Arul | London |
| 2 | John | Manchester |
| 3 | Priya | London |
| 4 | Sara | Birmingham |

## Answer

```sql
SELECT CustomerName, City
FROM Customers
WHERE City = 'Birmingham';
```

## Expected Result

| CustomerName | City |
|---|---|
| Sara | Birmingham |
