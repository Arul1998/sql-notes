# Lesson 64: TRIM Function

`TRIM` removes spaces from the beginning and end of text.

It does not remove spaces between words.

## Sample Table

Imagine this `Customers` table:

| CustomerId | CustomerName | City |
|---:|---|---|
| 1 |   Sarah   | London |
| 2 |  David | NULL |
| 3 | Priya  | Chennai |

## Syntax

```sql
TRIM(column_name)
```

## Example

```sql
SELECT CustomerName,
       TRIM(CustomerName) AS CleanName
FROM Customers;
```

## Exercise

Display `CustomerName` and `CleanName`.

Use `TRIM` to remove spaces from the beginning and end of `CustomerName`.
