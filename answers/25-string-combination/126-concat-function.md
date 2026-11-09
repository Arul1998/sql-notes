# Lesson 126 Answer: CONCAT

## Exercise

Using the `Customers` table, write a query to return `CustomerId` and `CustomerDetails`. Use `CONCAT()` to combine `FirstName`, one space, `LastName`, the separator `' - '`, and `City`.

## Sample Table

**Customers**

| CustomerId | FirstName | LastName | City |
|---:|---|---|---|
| 1 | Arun | Kumar | Chennai |
| 2 | Priya | Sharma | Mumbai |
| 3 | James | Brown | London |

## Answer

```sql
SELECT
    CustomerId,
    CONCAT(FirstName, ' ', LastName, ' - ', City) AS CustomerDetails
FROM Customers;
```

## Expected Result

| CustomerId | CustomerDetails |
|---:|---|
| 1 | Arun Kumar - Chennai |
| 2 | Priya Sharma - Mumbai |
| 3 | James Brown - London |
