# Lesson 138 Answer: DATALENGTH

## Exercise

Using `Customers`, display `CustomerId`, `CustomerName`, and `NameBytes`. Use `DATALENGTH()` to count the bytes in each `NVARCHAR(50)` customer name.

## Sample Table

`CustomerName` has data type `NVARCHAR(50)`.

| CustomerId | CustomerName |
|---:|---|
| 1 | Arun |
| 2 | Priya |
| 3 | Christopher |
| 4 | James |

## Answer

```sql
SELECT
    CustomerId,
    CustomerName,
    DATALENGTH(CustomerName) AS NameBytes
FROM Customers;
```

## Expected Result

| CustomerId | CustomerName | NameBytes |
|---:|---|---:|
| 1 | Arun | 8 |
| 2 | Priya | 10 |
| 3 | Christopher | 22 |
| 4 | James | 10 |
