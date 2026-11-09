# Lesson 137 Answer: LEN

## Exercise

Using `Customers`, display `CustomerId`, `CustomerName`, and `NameLength`. Use `LEN()` to count the characters in each customer name.

## Sample Table

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
    LEN(CustomerName) AS NameLength
FROM Customers;
```

## Expected Result

| CustomerId | CustomerName | NameLength |
|---:|---|---:|
| 1 | Arun | 4 |
| 2 | Priya | 5 |
| 3 | Christopher | 11 |
| 4 | James | 5 |
