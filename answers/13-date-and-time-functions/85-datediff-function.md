# Lesson 85 Answer: DATEDIFF Function

## Exercise

Find the difference in days between `OrderDate` and `DeliveryDate` and name it `DaysTaken`.

## Sample Table

| OrderId | OrderDate | DeliveryDate |
|---:|---|---|
| 101 | 2026-08-01 | 2026-08-05 |
| 102 | 2026-08-03 | 2026-08-10 |

## Answer

```sql
SELECT OrderId, OrderDate, DeliveryDate,
       DATEDIFF(DAY, OrderDate, DeliveryDate) AS DaysTaken
FROM Orders;
```

## Expected Result

| OrderId | OrderDate | DeliveryDate | DaysTaken |
|---:|---|---|---:|
| 101 | 2026-08-01 | 2026-08-05 | 4 |
| 102 | 2026-08-03 | 2026-08-10 | 7 |
