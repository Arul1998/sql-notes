# Lesson 21 Answer: Table Aliases

## Exercise

Using aliases `c` and `o`, display `CustomerName`, `OrderId`, and `Amount`. Show only orders below £300 and sort them from the highest amount to the lowest.

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
    o.OrderId,
    o.Amount
FROM Customers AS c
INNER JOIN Orders AS o
    ON c.CustomerId = o.CustomerId
WHERE o.Amount < 300
ORDER BY o.Amount DESC;
```

## Expected Result

| CustomerName | OrderId | Amount |
|---|---:|---:|
| Arul | 101 | 200 |
| Arul | 103 | 150 |
