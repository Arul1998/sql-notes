# Lesson 71: SPACE Function

`SPACE` returns a specified number of spaces.

It is useful when joining text values.

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
SPACE(number_of_spaces)
```

## Example

```sql
SELECT CONCAT(CustomerName, SPACE(1), Country) AS CustomerDetails
FROM Customers;
```

## Exercise

Display a calculated column named `CustomerDetails`.

Use `CONCAT` and `SPACE` to join `CustomerName`, two spaces, and `City`.
