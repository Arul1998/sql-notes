# Lesson 22: LEFT JOIN

`LEFT JOIN` returns every row from the left table and matching rows from the right table.

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

To display every customer, including customers without orders:

```sql
SELECT
    c.CustomerName,
    o.OrderId,
    o.Amount
FROM Customers AS c
LEFT JOIN Orders AS o
    ON c.CustomerId = o.CustomerId;
```

Sara appears with `NULL` values because she has no matching order.

To find only customers without orders:

```sql
SELECT c.CustomerName
FROM Customers AS c
LEFT JOIN Orders AS o
    ON c.CustomerId = o.CustomerId
WHERE o.OrderId IS NULL;
```

## Exercise

Using `LEFT JOIN`, display only customers who have never placed an order. Return `CustomerName`.
