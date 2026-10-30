# Lesson 111: OUTPUT with DELETE

`OUTPUT DELETED` shows values from deleted rows.

## Sample Table

| OrderId | CustomerId | Amount | Status |
|---:|---:|---:|---|
| 101 | 1 | 250 | Pending |
| 102 | 1 | 400 | Shipped |
| 103 | 2 | 150 | Pending |

## Syntax

```sql
DELETE FROM table OUTPUT DELETED.column WHERE condition;
```

## Example

```sql
DELETE
FROM Orders
OUTPUT DELETED.OrderId, DELETED.Amount
WHERE Status = 'Pending';
```

## Exercise

Delete pending orders and return the deleted OrderId and Amount.
