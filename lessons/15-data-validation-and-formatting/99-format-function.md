# Lesson 99: FORMAT Function

`FORMAT` displays a value using a specified format.

## Sample Table

Imagine this `Orders` table:

| OrderId | OrderDate |
|---:|---|
| 101 | 2026-08-12 |
| 102 | 2026-12-25 |

## Syntax

```sql
FORMAT(value, format)
```

## Example

```sql
SELECT OrderId,
       FORMAT(OrderDate, 'dd/MM/yyyy') AS FormattedDate
FROM Orders;
```

## Exercise

Display `OrderId`, `OrderDate`, and format `OrderDate` as `dd/MM/yyyy`.

Name the new column `FormattedOrderDate`.
