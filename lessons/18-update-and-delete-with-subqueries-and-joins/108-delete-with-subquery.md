# Lesson 108: DELETE with Subquery

A subquery can identify which rows to delete.

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

## Syntax

```sql
DELETE FROM table WHERE column IN (SELECT column FROM other_table WHERE condition);
```

## Example

```sql
DELETE
FROM Orders
WHERE CustomerId IN (SELECT CustomerId
FROM Customers
WHERE CustomerName = 'Sarah');
```

## Exercise

Delete orders belonging to customers whose name is Sarah.
