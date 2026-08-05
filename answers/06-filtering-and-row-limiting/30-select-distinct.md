# Lesson 30 Answer: Selecting Distinct Values

## Exercise

Display each different `CustomerId` from the `Orders` table.

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
SELECT DISTINCT CustomerId
FROM Orders;
```

## Expected Result

### Result

| CustomerId |
|---:|
| 1 |
| 2 |
| 3 |
| 4 |