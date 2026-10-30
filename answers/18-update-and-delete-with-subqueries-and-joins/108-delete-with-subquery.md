# Lesson 108 Answer: DELETE with Subquery

## Exercise

Delete orders belonging to customers whose name is Sarah.

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
DELETE
FROM Orders
WHERE CustomerId IN (SELECT CustomerId
FROM Customers
WHERE CustomerName = 'Sarah');
```

## Expected Result

| OrderId | CustomerId | Amount | Status |
|---:|---:|---:|---|
| 101 | 1 | 250 | Pending |
| 102 | 1 | 400 | Shipped |
