# Lesson 73: STUFF Function

`STUFF` removes part of a string and inserts new text at the same position.

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
STUFF(text, start_position, number_to_delete, replacement_text)
```

## Example

```sql
SELECT STUFF('Sarah', 2, 2, 'XX') AS UpdatedName;
```

## Exercise

Display `CustomerName` and `HiddenName`.

Replace the first three characters of each name with `***`.
