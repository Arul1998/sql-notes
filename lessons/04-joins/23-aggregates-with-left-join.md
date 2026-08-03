# Lesson 23: Aggregates with LEFT JOIN

Aggregate functions can calculate results after a `LEFT JOIN`.

Imagine these tables:

**Customers**

| CustomerId | CustomerName |
|---:|---|
| 1 | Arul |
| 2 | Priya |
| 3 | John |
| 4 | Sara |

**Orders**

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 200 |
| 102 | 2 | 350 |
| 103 | 1 | 150 |
| 104 | 3 | 500 |

To count each customer's orders:

```sql
SELECT
    c.CustomerName,
    COUNT(o.OrderId) AS OrderCount
FROM Customers AS c
LEFT JOIN Orders AS o
    ON c.CustomerId = o.CustomerId
GROUP BY c.CustomerId, c.CustomerName;
```

Use `COUNT(o.OrderId)`, not `COUNT(*)`. For customers without orders:

- `COUNT(o.OrderId)` returns 0.
- `COUNT(*)` would return 1 because the customer row still exists.

To replace a missing total with zero, SQL Server can use `COALESCE`:

```sql
COALESCE(SUM(o.Amount), 0)
```

## Exercise

Display every customer and their total order amount. Name the calculated column `TotalAmount`. Customers without orders should also appear.
