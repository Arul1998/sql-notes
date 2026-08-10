# Lesson 63: LOWER Function

`LOWER` converts text to lowercase letters.

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
LOWER(column_name)
```

## Example

```sql
SELECT City,
       LOWER(City) AS LowercaseCity
FROM Customers;
```

## Exercise

Display `CustomerName` and `LowercaseName`.

Use `LOWER` on each customer name.
