# Lesson 68: REPLACE Function

`REPLACE` finds text inside a string and replaces every match with different text.

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
REPLACE(column_name, text_to_find, replacement_text)
```

## Example

```sql
SELECT City,
       REPLACE(City, 'Manchester', 'Greater Manchester') AS UpdatedCity
FROM Customers;
```

## Exercise

Display `CustomerName`, `City`, and `UpdatedCity`.

Change `London` to `Greater London` in the `City` column.
