# Lesson 112 Answer: OUTPUT with UPDATE

## Exercise

Update OrderId 101 by increasing Amount by 50. Return old and new amounts.

## Sample Table

| OrderId | Amount |
|---:|---:|
| 101 | 250 |
| 102 | 400 |

## Answer

```sql
UPDATE Orders SET Amount = Amount + 50
OUTPUT DELETED.Amount AS OldAmount, INSERTED.Amount AS NewAmount
WHERE OrderId = 101;
```

## Expected Result

| OldAmount | NewAmount |
|---:|---:|
| 250 | 300 |
