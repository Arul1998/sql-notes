# Lesson 110: DELETE with JOIN

`DELETE ... FROM JOIN` deletes matching rows from the target table.

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
DELETE t FROM table AS t INNER JOIN other_table AS x ON t.Id = x.Id WHERE condition;
```

## Example

```sql
DELETE o
FROM Orders AS o
INNER JOIN Customers AS c ON c.CustomerId = o.CustomerId
WHERE c.CustomerName = 'Sarah';
```

## Exercise

Delete orders placed by customer Sarah.
