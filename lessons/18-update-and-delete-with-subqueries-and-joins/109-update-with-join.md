# Lesson 109: UPDATE with JOIN

`UPDATE ... FROM JOIN` updates rows based on a matching table.

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
UPDATE t SET t.column = value FROM table AS t INNER JOIN other_table AS x ON t.Id = x.Id WHERE condition;
```

## Example

```sql
UPDATE o SET o.Amount = o.Amount + 50
FROM Orders AS o
INNER JOIN Customers AS c ON c.CustomerId = o.CustomerId
WHERE c.CustomerName = 'John';
```

## Exercise

Increase the Amount by 50 for orders belonging to customer John.
