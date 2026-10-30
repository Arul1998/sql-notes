# Lesson 105 Answer: SELECT INTO

## Exercise

Create a new table called HighValueOrders containing orders with Amount greater than 200.

## Sample Table

| OrderId | CustomerId | Amount | Status |
|---:|---:|---:|---|
| 101 | 1 | 250 | Pending |
| 102 | 1 | 400 | Shipped |
| 103 | 2 | 150 | Pending |

## Answer

```sql
SELECT OrderId, CustomerId, Amount, Status
INTO HighValueOrders
FROM Orders
WHERE Amount > 200;
```

## Expected Result

| OrderId | CustomerId | Amount | Status |
|---:|---:|---:|---|
| 101 | 1 | 250 | Pending |
| 102 | 1 | 400 | Shipped |
