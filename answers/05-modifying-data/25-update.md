# Lesson 25 Answer: UPDATE

## Exercise

Change the amount of order 102 to 400.

## Sample Table

### Orders Before UPDATE

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 200 |
| 102 | 2 | 350 |
| 103 | 1 | 150 |
| 104 | 3 | 500 |
| 105 | 4 | 250 |

## Answer

```sql
UPDATE Orders
SET Amount = 400
WHERE OrderId = 102;
```

## Expected Result

### Orders After UPDATE

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 200 |
| 102 | 2 | 400 |
| 103 | 1 | 150 |
| 104 | 3 | 500 |
| 105 | 4 | 250 |
