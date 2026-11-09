# Lesson 141: RTRIM

`RTRIM()` removes trailing spaces from the right side of a string, leaving leading spaces unchanged.

## Sample Table

Quotation marks show spaces and are not part of the stored values.

| CustomerId | CustomerName | City |
|---:|---|---|
| 1 | `'Arun   '` | Chennai |
| 2 | `'  Priya  '` | Mumbai |
| 3 | `'James Brown    '` | London |
| 4 | `' Christopher '` | Manchester |

## Syntax

```sql
RTRIM(text)
```

## Example

```sql
SELECT RTRIM('   Hello SQL   ') AS CleanText;
```

## Exercise

Using `Customers`, display `CustomerId`, `RTRIM(CustomerName)` as `CleanCustomerName`, and `City`. Remove only trailing spaces and preserve leading spaces.
