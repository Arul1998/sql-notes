# Lesson 102: NOT EXISTS

`NOT EXISTS` returns rows when the subquery finds no matching rows.

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

## Syntax

```sql
SELECT columns FROM table1 WHERE NOT EXISTS (SELECT 1 FROM table2 WHERE matching_condition);
```

## Example

```sql
SELECT c.CustomerId, c.CustomerName
FROM Customers AS c
WHERE NOT EXISTS (
    SELECT 1
    FROM Orders AS o
    WHERE o.CustomerId = c.CustomerId
);
```

## Exercise

Find customers who have no orders.
