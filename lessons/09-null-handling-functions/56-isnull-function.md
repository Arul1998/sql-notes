# Lesson 56: ISNULL Function

`ISNULL` replaces a `NULL` value with another value.

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
ISNULL(column_name, replacement_value)
```

## Example

```sql
SELECT CustomerName,
       ISNULL(Country, 'Unknown') AS DisplayCountry
FROM Customers;
```

## Exercise

Display `CustomerName`, `City`, and `DisplayCity` from `Customers`.

If `City` is `NULL`, display `Unknown`. Otherwise, display the original city.
