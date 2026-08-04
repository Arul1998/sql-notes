# Lesson 22 Answer: LEFT JOIN

## Exercise

Using `LEFT JOIN`, display only customers who have never placed an order. Return `CustomerName`.

## Sample Table

### Customers

| CustomerId | CustomerName |
|---:|---|
| 1 | Arul |
| 2 | Priya |
| 3 | John |
| 4 | Sara |

### Orders

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 200 |
| 102 | 2 | 350 |
| 103 | 1 | 150 |
| 104 | 3 | 500 |

## Answer

```sql
SELECT c.CustomerName
FROM Customers AS c
LEFT JOIN Orders AS o
    ON c.CustomerId = o.CustomerId
WHERE o.OrderId IS NULL;
```

## Expected Result

| CustomerName |
|---|
| Sara |
