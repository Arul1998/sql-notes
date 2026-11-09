# Lesson 127: CONCAT_WS

`CONCAT_WS()` combines values using a separator supplied once as its first argument. It skips `NULL` values.

## Sample Table

| CustomerId | FirstName | LastName | City | Country |
|---:|---|---|---|---|
| 1 | Arun | Kumar | Chennai | India |
| 2 | Priya | Sharma | Mumbai | India |
| 3 | James | Brown | London | UK |

## Syntax

```sql
CONCAT_WS(separator, value1, value2, ...)
```

## Example

```sql
SELECT CONCAT_WS(' - ', 'John', 'Smith', 'IT') AS EmployeeDetails;
```

## Exercise

Using the `Customers` table, return `CustomerId` and `CustomerInfo`. Join `FirstName`, `LastName`, `City`, and `Country` with a comma followed by one space using `CONCAT_WS()`.
