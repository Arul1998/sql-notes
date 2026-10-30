# Lesson 105: SELECT INTO

`SELECT INTO` creates a new table from the selected rows.

## Sample Table

| OrderId | CustomerId | Amount | Status |
|---:|---:|---:|---|
| 101 | 1 | 250 | Pending |
| 102 | 1 | 400 | Shipped |
| 103 | 2 | 150 | Pending |

## Syntax

```sql
SELECT columns INTO new_table FROM existing_table WHERE condition;
```

## Example

```sql
SELECT OrderId, CustomerId, Amount, Status
INTO HighValueOrders
FROM Orders
WHERE Amount > 200;
```

## Exercise

Create a new table called HighValueOrders containing orders with Amount greater than 200.
