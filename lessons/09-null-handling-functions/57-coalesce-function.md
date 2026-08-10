# Lesson 57: COALESCE Function

`COALESCE` returns the first value that is not `NULL`.

It checks values from left to right.

## Sample Table

Imagine this `Customers` table:

| CustomerId | CustomerName | City | Country |
|---:|---|---|---|
| 1 | Sarah | London | UK |
| 2 | David | NULL | UK |
| 3 | Priya | Chennai | India |
| 4 | James | Manchester | NULL |
| 5 | Amina | London | UK |

## Syntax

```sql
COALESCE(value1, value2, value3)
```

## Example

```sql
SELECT CustomerName,
       COALESCE(Country, 'Unknown') AS DisplayCountry
FROM Customers;
```

## Exercise

Display `CustomerName` and `ContactLocation` from `Customers`.

Return `City`, otherwise `Country`, otherwise `Unknown`.
