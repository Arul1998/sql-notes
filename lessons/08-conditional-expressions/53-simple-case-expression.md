# Lesson 53: Simple CASE Expression

A simple `CASE` compares one column with several exact values.

## Sample Table

Imagine this `Employees` table:

| EmployeeId | EmployeeName | Department | Salary |
|---:|---|---|---:|
| 1 | Sarah | IT | 55000 |
| 2 | David | HR | 42000 |
| 3 | Priya | Sales | 48000 |
| 4 | James | Finance | 38000 |
| 5 | Amina | NULL | 45000 |

## Syntax

```sql
CASE column_name
    WHEN value1 THEN result1
    WHEN value2 THEN result2
    ELSE other_result
END
```

## Example

```sql
SELECT EmployeeName,
       CASE Department
           WHEN 'IT' THEN 'Technology Team'
           WHEN 'HR' THEN 'People Team'
           ELSE 'Other Team'
       END AS TeamName
FROM Employees;
```

## Exercise

Display `EmployeeName`, `Department`, and `DepartmentName` from `Employees`.

- `IT` becomes `Technology`.
- `HR` becomes `Human Resources`.
- `Sales` becomes `Sales Team`.
- Anything else becomes `Other`.
