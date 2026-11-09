# Lesson 140: LTRIM

`LTRIM()` removes leading spaces from the left side of a string, leaving trailing spaces unchanged.

## Sample Table

Quotation marks show spaces and are not part of the stored values.

| CustomerId | CustomerName | City |
|---:|---|---|
| 1 | `'   Arun'` | Chennai |
| 2 | `'  Priya  '` | Mumbai |
| 3 | `'    James Brown'` | London |
| 4 | `' Christopher '` | Manchester |

## Syntax

```sql
LTRIM(text)
```

## Example

```sql
SELECT LTRIM('   Hello SQL   ') AS CleanText;
```

## Exercise

Using `Customers`, display `CustomerId`, `LTRIM(CustomerName)` as `CleanCustomerName`, and `City`. Remove only leading spaces and preserve trailing spaces.
