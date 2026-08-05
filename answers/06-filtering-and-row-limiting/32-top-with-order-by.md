# Lesson 32 Answer: TOP with ORDER BY

## Exercise

Display the 2 orders with the lowest `Amount`.

## Sample Table

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 200 |
| 102 | 2 | 350 |
| 103 | 1 | 150 |
| 104 | 3 | 500 |
| 105 | 4 | 250 |

## Answer

```sql
SELECT TOP (2) *
FROM Orders
ORDER BY Amount ASC;
```

## Expected Result

### Result

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 103 | 1 | 150 |
| 101 | 1 | 200 |