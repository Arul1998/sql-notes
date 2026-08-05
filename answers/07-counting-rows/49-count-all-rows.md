# Lesson 49 Answer: Counting All Rows

## Exercise

Count all rows in the `Orders` table.

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
SELECT COUNT(*)
FROM Orders;
```

## Expected Result

### Result

| (No column name) |
|---:|
| 5 |