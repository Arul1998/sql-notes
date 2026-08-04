# Lesson 14 Answer: SUM and AVG

## Exercise

Calculate the total and average salary of employees in the IT department. Name the columns `ITTotalSalary` and `ITAverageSalary`.

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
    SUM(Salary) AS ITTotalSalary,
    AVG(Salary) AS ITAverageSalary
FROM Employees
WHERE Department = 'IT';
```

## Expected Result

| ITTotalSalary | ITAverageSalary |
|---:|---:|
| 66000 | 33000 |
