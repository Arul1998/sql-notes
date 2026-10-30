# Lesson 120: IIF

`IIF` returns one value if a condition is true and another if false.

## Sample Table

| EmployeeName | Salary |
|---|---:|
| John | 40000 |
| Sarah | 50000 |
| David | 30000 |

## Syntax

```sql
IIF(condition, true_value, false_value)
```

## Example

```sql
SELECT EmployeeName, IIF(Salary >= 40000, 'High', 'Low') AS SalaryLevel
FROM Employees;
```

## Exercise

Display EmployeeName and SalaryLevel ('High' for Salary at least 40000, otherwise 'Low').
