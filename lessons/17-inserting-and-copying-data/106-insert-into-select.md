# Lesson 106: INSERT INTO SELECT

`INSERT INTO SELECT` copies query results into an existing table.

## Sample Table

| OrderId | CustomerId | Amount | Status |
|---:|---:|---:|---|
| 101 | 1 | 250 | Pending |
| 102 | 1 | 400 | Shipped |
| 103 | 2 | 150 | Pending |

## Syntax

```sql
INSERT INTO target_table (columns) SELECT columns FROM source_table WHERE condition;
```

## Example

```sql
INSERT
INTO HighValueOrders (OrderId, CustomerId, Amount, Status) SELECT OrderId, CustomerId, Amount, Status
FROM Orders
WHERE Amount > 200;
```

## Exercise

Copy orders with Amount greater than 200 from Orders into an existing table called HighValueOrders with the same columns.
