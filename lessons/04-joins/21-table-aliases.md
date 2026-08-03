# Lesson 21: Table Aliases

Table aliases give tables shorter names inside a query.

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

Use `c` for `Customers` and `o` for `Orders`:

```sql
SELECT
    c.CustomerName,
    o.OrderId,
    o.Amount
FROM Customers AS c
INNER JOIN Orders AS o
    ON c.CustomerId = o.CustomerId;
```

- `c` represents `Customers`.
- `o` represents `Orders`.
- `AS` is optional for table aliases.

## Exercise

Using aliases `c` and `o`, display `CustomerName`, `OrderId`, and `Amount`. Show only orders below £300 and sort them from the highest amount to the lowest.
