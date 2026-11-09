# Lesson 139: TRIM

`TRIM()` removes spaces from both the beginning and end of a string, while keeping spaces between words. It is available in SQL Server 2017 and later.

## Sample Table

Quotation marks show spaces and are not part of the stored values.

| CustomerId | CustomerName | City |
|---:|---|---|
| 1 | `'  Arun  '` | Chennai |
| 2 | `' Priya '` | Mumbai |
| 3 | `'   James Brown   '` | London |
| 4 | `' Christopher  '` | Manchester |

## Syntax

```sql
TRIM(text)
```

## Example

```sql
SELECT TRIM('   Hello SQL   ') AS CleanText;
```

## Exercise

Using `Customers`, display `CustomerId`, `TRIM(CustomerName)` as `CleanCustomerName`, and `City`. Remove both leading and trailing spaces without changing the table.
