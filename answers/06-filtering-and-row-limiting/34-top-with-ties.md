# Lesson 34 Answer: TOP with TIES

## Exercise

Display the top 3 orders by `Amount`, including tied rows.

## Sample Table

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 500 |
| 102 | 2 | 450 |
| 103 | 1 | 400 |
| 104 | 3 | 400 |
| 105 | 4 | 250 |

## Answer

```sql
SELECT TOP (3) WITH TIES *
FROM Orders
ORDER BY Amount DESC;
```

## Expected Result

### Result

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 500 |
| 102 | 2 | 450 |
| 103 | 1 | 400 |
| 104 | 3 | 400 |