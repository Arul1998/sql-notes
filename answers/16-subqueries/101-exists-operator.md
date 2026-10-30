# Lesson 101 Answer: EXISTS Operator

## Exercise

Write a query to display `EmployeeId` and `EmployeeName` from `Employees`, but only for employees who have at least one record in `Orders`.

Use `EXISTS`.

## Sample Tables

**Employees**

| EmployeeId | EmployeeName |
|---:|---|
| 1 | John |
| 2 | Sarah |
| 3 | David |

**Orders**

| OrderId | EmployeeId | Amount |
|---:|---:|---:|
| 101 | 1 | 250 |
| 102 | 1 | 400 |
| 103 | 3 | 150 |

## Answer

```sql
SELECT EmployeeId, EmployeeName
FROM Employees AS e
WHERE EXISTS (
    SELECT 1
    FROM Orders AS o
    WHERE o.EmployeeId = e.EmployeeId
);
```

## Expected Result

| EmployeeId | EmployeeName |
|---:|---|
| 1 | John |
| 3 | David |
