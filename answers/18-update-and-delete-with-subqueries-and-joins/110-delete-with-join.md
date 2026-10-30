# Lesson 110 Answer: DELETE with JOIN

## Exercise

Delete orders placed by customer Sarah.

## Sample Tables

| OrderId | CustomerId | Amount | Status |
|---:|---:|---:|---|
| 101 | 1 | 250 | Pending |
| 102 | 1 | 400 | Shipped |
| 103 | 2 | 150 | Pending |

**Customers**

| CustomerId | CustomerName |
|---:|---|
| 1 | John |
| 2 | Sarah |
| 3 | David |

## Answer

```sql
DELETE o
FROM Orders AS o
INNER JOIN Customers AS c ON c.CustomerId = o.CustomerId
WHERE c.CustomerName = 'Sarah';
```

## Expected Result

| OrderId | CustomerId | Amount | Status |
|---:|---:|---:|---|
| 101 | 1 | 250 | Pending |
| 102 | 1 | 400 | Shipped |
