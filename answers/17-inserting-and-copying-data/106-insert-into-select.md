# Lesson 106 Answer: INSERT INTO SELECT

## Exercise

Copy orders with Amount greater than 200 from Orders into an existing table called HighValueOrders with the same columns.

## Sample Table

| OrderId | CustomerId | Amount | Status |
|---:|---:|---:|---|
| 101 | 1 | 250 | Pending |
| 102 | 1 | 400 | Shipped |
| 103 | 2 | 150 | Pending |

## Answer

```sql
INSERT
INTO HighValueOrders (OrderId, CustomerId, Amount, Status) SELECT OrderId, CustomerId, Amount, Status
FROM Orders
WHERE Amount > 200;
```

## Expected Result

| OrderId | CustomerId | Amount | Status |
|---:|---:|---:|---|
| 101 | 1 | 250 | Pending |
| 102 | 1 | 400 | Shipped |
