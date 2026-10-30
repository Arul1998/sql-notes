# Lesson 102 Answer: NOT EXISTS

## Exercise

Find customers who have no orders.

## Sample Tables

| CustomerId | CustomerName |
|---:|---|
| 1 | John |
| 2 | Sarah |
| 3 | David |

**Orders**

| OrderId | CustomerId | Amount | Status |
|---:|---:|---:|---|
| 101 | 1 | 250 | Pending |
| 102 | 1 | 400 | Shipped |
| 103 | 2 | 150 | Pending |

## Answer

```sql
SELECT c.CustomerId, c.CustomerName
FROM Customers AS c
WHERE NOT EXISTS (
    SELECT 1
    FROM Orders AS o
    WHERE o.CustomerId = c.CustomerId
);
```

## Expected Result

| CustomerId | CustomerName |
|---:|---|
| 3 | David |
