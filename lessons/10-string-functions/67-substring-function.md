# Lesson 67: SUBSTRING Function

`SUBSTRING` returns part of a string from a chosen position.

SQL Server starts counting from `1`.

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
SUBSTRING(column_name, start_position, number_of_characters)
```

## Example

```sql
SELECT CustomerName,
       SUBSTRING(CustomerName, 1, 3) AS NamePart
FROM Customers;
```

## Exercise

Display `CustomerName` and `NamePart`.

Return three characters starting from the second character.
