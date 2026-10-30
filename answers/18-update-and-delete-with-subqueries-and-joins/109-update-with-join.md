# Lesson 109 Answer: UPDATE with JOIN

## Exercise

Increase the Amount by 50 for orders belonging to customer John.

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
UPDATE o SET o.Amount = o.Amount + 50
FROM Orders AS o
INNER JOIN Customers AS c ON c.CustomerId = o.CustomerId
WHERE c.CustomerName = 'John';
```

## Expected Result

| OrderId | CustomerId | Amount | Status |
|---:|---:|---:|---|
| 101 | 1 | 300 | Pending |
| 102 | 1 | 450 | Shipped |
| 103 | 2 | 150 | Pending |
