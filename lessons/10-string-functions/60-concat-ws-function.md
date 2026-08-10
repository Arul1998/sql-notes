# Lesson 60: CONCAT_WS Function

`CONCAT_WS` joins values using one separator.

It skips `NULL` values.

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
CONCAT_WS(separator, value1, value2, value3)
```

## Example

```sql
SELECT CONCAT_WS(' - ', CustomerName, City) AS CustomerDetails
FROM Customers;
```

## Exercise

Display `CustomerName`, `City`, `Country`, and `FullLocation`.

Join the three values with a comma followed by a space.
