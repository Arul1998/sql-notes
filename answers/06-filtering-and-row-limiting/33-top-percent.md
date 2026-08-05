# Lesson 33 Answer: Selecting TOP PERCENT

## Exercise

Display the top 25 percent of rows from `Employees`.

## Sample Table

| EmployeeId | EmployeeName | Department | Salary |
|---:|---|---|---:|
| 1 | Arul | IT | 36000 |
| 2 | Priya | HR | 45000 |
| 3 | John | IT | 30000 |
| 4 | Sara | Finance | 52000 |
| 5 | Adam | Sales | 34000 |
| 6 | Maya | NULL | 41000 |

## Answer

```sql
SELECT TOP (25) PERCENT *
FROM Employees;
```

## Expected Result

With 6 employees, SQL Server returns 2 rows because 25 percent of 6 is 1.5 and the result is rounded up.