# Lesson 38 Answer: Filtering with BETWEEN

## Exercise

Display orders with an `Amount` between 250 and 400.

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
SELECT *
FROM Orders
WHERE Amount BETWEEN 250 AND 400;
```

## Expected Result

### Result

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 102 | 2 | 350 |
| 105 | 4 | 250 |