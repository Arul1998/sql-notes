# Lesson 69: CHARINDEX Function

`CHARINDEX` returns the starting position of text inside another string.

It returns `0` when the text is not found.

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
CHARINDEX(text_to_find, column_name)
```

## Example

```sql
SELECT CustomerName,
       CHARINDEX('r', CustomerName) AS LetterPosition
FROM Customers;
```

## Exercise

Display `CustomerName` and `LetterPosition`.

Find the position of the first letter `a` in each name.
