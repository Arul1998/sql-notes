# Lesson 66: RIGHT Function

`RIGHT` returns a specified number of characters from the end of a string.

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
RIGHT(column_name, number_of_characters)
```

## Example

```sql
SELECT CustomerName,
       RIGHT(CustomerName, 3) AS LastThreeLetters
FROM Customers;
```

## Exercise

Display `CustomerName` and `LastTwoLetters`.

Use `RIGHT` to return the last two characters.
