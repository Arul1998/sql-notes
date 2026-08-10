# Lesson 62: UPPER Function

`UPPER` converts text to uppercase letters.

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
UPPER(column_name)
```

## Example

```sql
SELECT City,
       UPPER(City) AS UppercaseCity
FROM Customers;
```

## Exercise

Display `CustomerName` and `UppercaseName`.

Use `UPPER` on each customer name.
