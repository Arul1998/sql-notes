# Lesson 40: Filtering with IN

`IN` checks whether a value matches any value in a list.

## Sample Table

| EmployeeId | EmployeeName | Department | Salary |
|---:|---|---|---:|
| 1 | Arul | IT | 36000 |
| 2 | Priya | HR | 45000 |
| 3 | John | IT | 30000 |
| 4 | Sara | Finance | 52000 |
| 5 | Adam | Sales | 34000 |
| 6 | Maya | NULL | 41000 |

## Syntax

```sql
SELECT columns
FROM table_name
WHERE column_name IN (value1, value2, value3);
```

## Example

```sql
SELECT *
FROM Employees
WHERE Department IN ('IT', 'HR', 'Sales');
```

`IN` is shorter and clearer than writing several `OR` conditions.

## Exercise

Display employees in the `IT` or `Finance` departments.