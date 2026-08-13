# Lesson 88: EOMONTH Function

`EOMONTH` returns the last date of the month for a given date.

## Sample Table

Imagine this `Orders` table:

| OrderId | OrderDate |
|---:|---|
| 101 | 2026-08-10 |
| 102 | 2026-02-10 |

## Syntax

```sql
EOMONTH(date)
```

## Example

```sql
SELECT OrderId,
       EOMONTH(OrderDate) AS MonthEnd
FROM Orders;
```

## Exercise

Display `OrderId`, `OrderDate`, and the last day of the month containing `OrderDate`.

Name the new column `LastDayOfMonth`.
