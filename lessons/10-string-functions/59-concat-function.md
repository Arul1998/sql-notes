# Lesson 59: CONCAT Function

`CONCAT` joins two or more values into one string.

It treats a `NULL` value as an empty string.

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
CONCAT(value1, value2, value3)
```

## Example

```sql
SELECT CustomerName,
       CONCAT(CustomerName, ' - ', Country) AS CustomerDetails
FROM Customers;
```

## Exercise

Display `CustomerName`, `City`, and `CustomerLocation` from `Customers`.

Join the name and city in this format: `Sarah - London`.
