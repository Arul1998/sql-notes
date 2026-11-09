# Lesson 139 Answer: TRIM

## Exercise

Using `Customers`, display `CustomerId`, `TRIM(CustomerName)` as `CleanCustomerName`, and `City`. Remove both leading and trailing spaces without changing the table.

## Sample Table

Quotation marks show spaces and are not part of the stored values.

| CustomerId | CustomerName | City |
|---:|---|---|
| 1 | `'  Arun  '` | Chennai |
| 2 | `' Priya '` | Mumbai |
| 3 | `'   James Brown   '` | London |
| 4 | `' Christopher  '` | Manchester |

## Answer

```sql
SELECT
    CustomerId,
    TRIM(CustomerName) AS CleanCustomerName,
    City
FROM Customers;
```

## Expected Result

| CustomerId | CleanCustomerName | City |
|---:|---|---|
| 1 | Arun | Chennai |
| 2 | Priya | Mumbai |
| 3 | James Brown | London |
| 4 | Christopher | Manchester |
