# Lesson 13 Answer: COUNT

## Exercise

Count employees whose salary is at least £40,000. Name the result column `HighSalaryEmployees`.

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
SELECT COUNT(*) AS HighSalaryEmployees
FROM Employees
WHERE Salary >= 40000;
```

## Expected Result

| HighSalaryEmployees |
|---:|
| 2 |
