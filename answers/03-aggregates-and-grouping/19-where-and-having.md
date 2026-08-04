# Lesson 19 Answer: WHERE and HAVING

## Exercise

Consider only employees earning at least £35,000. Display each department and its average salary, but only show departments whose average salary is greater than £40,000. Sort the results from the highest average salary to the lowest.

## Sample Table

### Employees

| EmployeeName | Department | Age | Salary |
|---|---|---:|---:|
| Arul | IT | 28 | 36000 |
| Priya | Finance | 32 | 45000 |
| John | IT | 25 | 30000 |
| Sara | Finance | 35 | 52000 |
| Adam | Sales | 29 | 34000 |

## Answer

```sql
SELECT
    Department,
    AVG(Salary) AS AverageSalary
FROM Employees
WHERE Salary >= 35000
GROUP BY Department
HAVING AVG(Salary) > 40000
ORDER BY AverageSalary DESC;
```

## Expected Result

| Department | AverageSalary |
|---|---:|
| Finance | 48500 |
