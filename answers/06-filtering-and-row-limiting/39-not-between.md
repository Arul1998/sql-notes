# Lesson 39 Answer: Filtering with NOT BETWEEN

## Exercise

Display orders whose `Amount` is not between 200 and 400.

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
WHERE Amount NOT BETWEEN 200 AND 400;
```

## Expected Result

### Result

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 103 | 1 | 150 |
| 104 | 3 | 500 |