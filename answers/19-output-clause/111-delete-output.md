# Lesson 111 Answer: OUTPUT with DELETE

## Exercise

Delete pending orders and return the deleted OrderId and Amount.

## Sample Table

| OrderId | CustomerId | Amount | Status |
|---:|---:|---:|---|
| 101 | 1 | 250 | Pending |
| 102 | 1 | 400 | Shipped |
| 103 | 2 | 150 | Pending |

## Answer

```sql
DELETE
FROM Orders
OUTPUT DELETED.OrderId, DELETED.Amount
WHERE Status = 'Pending';
```

## Expected Result

| OrderId | Amount |
|---:|---:|
| 101 | 250 |
| 103 | 150 |
