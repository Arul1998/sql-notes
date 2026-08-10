# Lesson 70: REVERSE Function

`REVERSE` returns the characters in a string in reverse order.

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
REVERSE(column_name)
```

## Example

```sql
SELECT City,
       REVERSE(City) AS ReversedCity
FROM Customers;
```

## Exercise

Display `CustomerName` and `ReversedName`.

Reverse each customer name.
