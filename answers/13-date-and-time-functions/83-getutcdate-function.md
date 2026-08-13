# Lesson 83 Answer: GETUTCDATE Function

## Exercise

Display `OrderId`, `Amount`, and the current UTC date and time.

Name the new column `UTCDateTime`.

## Sample Table

| OrderId | Amount |
|---:|---:|
| 101 | 125.20 |
| 102 | 250.75 |
| 103 | 399.10 |

## Answer

```sql
SELECT OrderId,
       Amount,
       GETUTCDATE() AS UTCDateTime
FROM Orders;
```

## Expected Result

`UTCDateTime` shows the current UTC date and time for each returned order.
