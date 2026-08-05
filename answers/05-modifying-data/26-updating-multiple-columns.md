# Lesson 26 Answer: Updating Multiple Columns

## Exercise

Update order 103:

- Change `CustomerId` to 2.
- Change `Amount` to 275.

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
SET CustomerId = 2,
    Amount = 275
WHERE OrderId = 103;
```

## Expected Result

### Orders After UPDATE

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 200 |
| 102 | 2 | 350 |
| 103 | 2 | 275 |
| 104 | 3 | 500 |
| 105 | 4 | 250 |
