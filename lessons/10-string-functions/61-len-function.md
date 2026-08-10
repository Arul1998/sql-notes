# Lesson 61: LEN Function

`LEN` returns the number of characters in a string, excluding trailing spaces.

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
LEN(column_name)
```

## Example

```sql
SELECT CustomerName,
       LEN(City) AS CityLength
FROM Customers;
```

## Exercise

Display `CustomerName` and `NameLength`.

Use `LEN` to count the characters in each customer name.
