# Lesson 65: LEFT Function

`LEFT` returns a specified number of characters from the beginning of a string.

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
LEFT(column_name, number_of_characters)
```

## Example

```sql
SELECT CustomerName,
       LEFT(CustomerName, 3) AS ShortName
FROM Customers;
```

## Exercise

Display `CustomerName` and `FirstTwoLetters`.

Use `LEFT` to return the first two characters.
