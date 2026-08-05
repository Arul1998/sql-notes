# Lesson 41: Filtering with NOT IN

`NOT IN` excludes rows whose value appears in a list.

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
WHERE column_name NOT IN (value1, value2);
```

## Example

```sql
SELECT *
FROM Employees
WHERE Department NOT IN ('HR', 'Sales');
```

Rows containing `NULL` in the tested column are not returned by this condition.

## Exercise

Display employees who are not in the `IT` or `HR` departments.