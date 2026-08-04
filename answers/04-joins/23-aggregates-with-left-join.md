# Lesson 23 Answer: Aggregates with LEFT JOIN

## Exercise

Display every customer and their total order amount. Name the calculated column `TotalAmount`. Customers without orders should also appear.

## Sample Table

### Customers

| CustomerId | CustomerName |
|---:|---|
| 1 | Arul |
| 2 | Priya |
| 3 | John |
| 4 | Sara |

### Orders

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 200 |
| 102 | 2 | 350 |
| 103 | 1 | 150 |
| 104 | 3 | 500 |

## Answer

```sql
SELECT
    c.CustomerName,
    COALESCE(SUM(o.Amount), 0) AS TotalAmount
FROM Customers AS c
LEFT JOIN Orders AS o
    ON c.CustomerId = o.CustomerId
GROUP BY c.CustomerId, c.CustomerName;
```

## Expected Result

| CustomerName | TotalAmount |
|---|---:|
| Arul | 350 |
| Priya | 350 |
| John | 500 |
| Sara | 0 |
