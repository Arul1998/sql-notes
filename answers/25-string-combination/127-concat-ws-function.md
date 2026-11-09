# Lesson 127 Answer: CONCAT_WS

## Exercise

Using the `Customers` table, return `CustomerId` and `CustomerInfo`. Join `FirstName`, `LastName`, `City`, and `Country` with a comma followed by one space using `CONCAT_WS()`.

## Sample Table

| CustomerId | FirstName | LastName | City | Country |
|---:|---|---|---|---|
| 1 | Arun | Kumar | Chennai | India |
| 2 | Priya | Sharma | Mumbai | India |
| 3 | James | Brown | London | UK |

## Answer

```sql
SELECT
    CustomerId,
    CONCAT_WS(', ', FirstName, LastName, City, Country) AS CustomerInfo
FROM Customers;
```

## Expected Result

| CustomerId | CustomerInfo |
|---:|---|
| 1 | Arun, Kumar, Chennai, India |
| 2 | Priya, Sharma, Mumbai, India |
| 3 | James, Brown, London, UK |
