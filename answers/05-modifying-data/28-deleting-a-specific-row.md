# Lesson 28 Answer: Deleting a Specific Row

## Exercise

Delete the order whose `OrderId` is 101.

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
DELETE FROM Orders
WHERE OrderId = 101;
```

## Expected Result

### Orders

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 102 | 2 | 350 |
| 103 | 1 | 150 |
| 104 | 3 | 500 |
| 105 | 4 | 250 |