# Lesson 126: CONCAT

`CONCAT()` combines two or more values into one string. It converts numbers to text automatically and treats `NULL` values as empty strings.

## Sample Tables

**Employees**

| EmployeeId | FirstName | LastName |
|---:|---|---|
| 1 | John | Smith |
| 2 | Sarah | Wilson |
| 3 | David | Brown |

**Customers**

| CustomerId | FirstName | LastName | City |
|---:|---|---|---|
| 1 | Arun | Kumar | Chennai |
| 2 | Priya | Sharma | Mumbai |
| 3 | James | Brown | London |

## Syntax

```sql
CONCAT(value1, value2, value3)
```

## Example

```sql
SELECT
    EmployeeId,
    CONCAT(FirstName, ' ', LastName) AS FullName
FROM Employees;
```

This joins each employee's first and last names with a space between them.

## Exercise

Using the `Customers` table, write a query to return `CustomerId` and `CustomerDetails`. Use `CONCAT()` to combine `FirstName`, one space, `LastName`, the separator `' - '`, and `City`.
