# Lesson 18 Answer: HAVING

## Exercise

Display each department and its average salary, but show only departments whose average salary is greater than £40,000. Name the calculated column `AverageSalary`.

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
GROUP BY Department
HAVING AVG(Salary) > 40000;
```

## Expected Result

| Department | AverageSalary |
|---|---:|
| Finance | 48500 |
