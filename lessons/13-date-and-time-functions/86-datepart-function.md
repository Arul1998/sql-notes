# Lesson 86: DATEPART Function

`DATEPART` extracts a specific part of a date as a number.

## Sample Table

Imagine this `Orders` table:

| OrderId | OrderDate |
|---:|---|
| 101 | 2026-08-10 |
| 102 | 2025-12-05 |

## Syntax

```sql
DATEPART(datepart, date)
```

## Example

```sql
SELECT OrderId,
       DATEPART(MONTH, OrderDate) AS OrderMonth
FROM Orders;
```

## Exercise

Display `OrderId`, `OrderDate`, and the year from `OrderDate`.

Name the new column `OrderYear`.
