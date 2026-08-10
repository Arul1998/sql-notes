# Lesson 53 Answer: Simple CASE Expression

## Exercise

Display `EmployeeName`, `Department`, and `DepartmentName` from `Employees`.

- `IT` becomes `Technology`.
- `HR` becomes `Human Resources`.
- `Sales` becomes `Sales Team`.
- Anything else becomes `Other`.

## Sample Table

| EmployeeId | EmployeeName | Department | Salary |
|---:|---|---|---:|
| 1 | Sarah | IT | 55000 |
| 2 | David | HR | 42000 |
| 3 | Priya | Sales | 48000 |
| 4 | James | Finance | 38000 |
| 5 | Amina | NULL | 45000 |

## Answer

```sql
SELECT EmployeeName,
       Department,
       CASE Department
           WHEN 'IT' THEN 'Technology'
           WHEN 'HR' THEN 'Human Resources'
           WHEN 'Sales' THEN 'Sales Team'
           ELSE 'Other'
       END AS DepartmentName
FROM Employees;
```

## Expected Result

### Result

| EmployeeName | Department | DepartmentName |
|---|---|---|
| Sarah | IT | Technology |
| David | HR | Human Resources |
| Priya | Sales | Sales Team |
| James | Finance | Other |
| Amina | NULL | Other |
