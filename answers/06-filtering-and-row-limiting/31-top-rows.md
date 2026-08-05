# Lesson 31 Answer: Selecting TOP Rows

## Exercise

Display the first 2 rows from `Orders`.

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
FROM Orders;
```

## Expected Result

### Result

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 200 |
| 102 | 2 | 350 |