# Lesson 55 Answer: CHOOSE Function

## Exercise

Display `OrderId` and `DeliveryType` from `Orders`.

Use `CHOOSE(1, 'Standard', 'Express', 'Collection')`.

## Sample Table

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 200 |
| 102 | 2 | 500 |
| 103 | 1 | 150 |
| 104 | 3 | 750 |
| 105 | 4 | 300 |

## Answer

```sql
SELECT OrderId,
       CHOOSE(1, 'Standard', 'Express', 'Collection') AS DeliveryType
FROM Orders;
```

## Expected Result

### Result

| OrderId | DeliveryType |
|---:|---|
| 101 | Standard |
| 102 | Standard |
| 103 | Standard |
| 104 | Standard |
| 105 | Standard |
