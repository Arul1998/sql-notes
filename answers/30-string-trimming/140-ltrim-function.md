# Lesson 140 Answer: LTRIM

## Exercise

Using `Customers`, display `CustomerId`, `LTRIM(CustomerName)` as `CleanCustomerName`, and `City`. Remove only leading spaces and preserve trailing spaces.

## Sample Table

Quotation marks show spaces and are not part of the stored values.

| CustomerId | CustomerName | City |
|---:|---|---|
| 1 | `'   Arun'` | Chennai |
| 2 | `'  Priya  '` | Mumbai |
| 3 | `'    James Brown'` | London |
| 4 | `' Christopher '` | Manchester |

## Answer

```sql
SELECT
    CustomerId,
    LTRIM(CustomerName) AS CleanCustomerName,
    City
FROM Customers;
```

## Expected Result

Quotation marks make remaining spaces visible.

| CustomerId | CleanCustomerName | City |
|---:|---|---|
| 1 | `'Arun'` | Chennai |
| 2 | `'Priya  '` | Mumbai |
| 3 | `'James Brown'` | London |
| 4 | `'Christopher '` | Manchester |
