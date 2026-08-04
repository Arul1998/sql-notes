# Lesson 20 Answer: INNER JOIN

## Exercise

Display `CustomerName` and `Amount` by joining `Customers` and `Orders`. Show only orders whose amount is at least £300.

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
    o.Amount
FROM Customers AS c
INNER JOIN Orders AS o
    ON c.CustomerId = o.CustomerId
WHERE o.Amount >= 300;
```

## Expected Result

| CustomerName | Amount |
|---|---:|
| Priya | 350 |
| John | 500 |
