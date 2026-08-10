# Lesson 72: REPLICATE Function

`REPLICATE` repeats text a specified number of times.

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
REPLICATE(text, number_of_times)
```

## Example

```sql
SELECT REPLICATE('*', 5) AS Symbols;
```

## Exercise

Display `CustomerName` and `NamePattern`.

Repeat each customer name three times.
