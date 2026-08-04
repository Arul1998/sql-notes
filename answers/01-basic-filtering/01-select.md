# Lesson 1 Answer: SELECT

## Exercise

Display only `CustomerId` and `CustomerName` from the `Customers` table.

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
SELECT CustomerId, CustomerName
FROM Customers;
```

## Expected Result

| CustomerId | CustomerName |
|---:|---|
| 1 | Arul |
| 2 | John |
| 3 | Priya |
| 4 | Sara |
