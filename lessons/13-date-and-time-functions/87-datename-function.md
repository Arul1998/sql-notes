# Lesson 87: DATENAME Function

`DATENAME` returns a selected part of a date as text.

It can return names such as a month name or weekday name.

## Sample Table

Imagine this `Orders` table:

| OrderId | OrderDate |
|---:|---|
| 101 | 2026-08-10 |
| 102 | 2026-08-11 |

## Syntax

```sql
DATENAME(datepart, date)
```

## Example

```sql
SELECT OrderId,
       DATENAME(MONTH, OrderDate) AS OrderMonth
FROM Orders;
```

## Exercise

Display `OrderId`, `OrderDate`, and the weekday name from `OrderDate`.

Name the new column `OrderDay`.
