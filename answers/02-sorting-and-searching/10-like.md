# Lesson 10 Answer: LIKE

## Exercise

Display `EmployeeName` and `Department` for employees whose name starts with S.

## Sample Table

### Employees

| EmployeeName | Department |
|---|---|
| Arul | IT |
| Priya | Finance |
| John | IT |
| Sara | Finance |
| Adam | Sales |

## Answer

```sql
SELECT EmployeeName, Department
FROM Employees
WHERE EmployeeName LIKE 'S%';
```

## Expected Result

| EmployeeName | Department |
|---|---|
| Sara | Finance |
