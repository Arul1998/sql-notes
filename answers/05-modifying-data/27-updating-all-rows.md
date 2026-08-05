# Lesson 27 Answer: Updating All Rows

## Exercise

Update all orders so that `Amount` becomes 500.

## Sample Table

### Orders Before UPDATE

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 200 |
| 102 | 2 | 350 |
| 103 | 1 | 150 |

## Answer

```sql
UPDATE Orders
SET Amount = 500;
```

## Expected Result

### Orders After UPDATE

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 500 |
| 102 | 2 | 500 |
| 103 | 1 | 500 |
