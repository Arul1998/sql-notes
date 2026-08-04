# Lesson 16 Answer: GROUP BY

## Exercise

Display each department and its average salary. Name the average column `AverageSalary`.

## Sample Table

### Employees

| EmployeeName | Department | Salary |
|---|---|---:|
| Arul | IT | 36000 |
| Priya | Finance | 45000 |
| John | IT | 30000 |
| Sara | Finance | 52000 |
| Adam | Sales | 34000 |

## Answer

```sql
SELECT
    Department,
    AVG(Salary) AS AverageSalary
FROM Employees
GROUP BY Department;
```

## Expected Result

| Department | AverageSalary |
|---|---:|
| IT | 33000 |
| Finance | 48500 |
| Sales | 34000 |
