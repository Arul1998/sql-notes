# Lesson 48: Finding Non-NULL Values

Use `IS NOT NULL` to find rows where a column contains a value.

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
WHERE column_name IS NOT NULL;
```

## Example

```sql
SELECT *
FROM Employees
WHERE Department IS NOT NULL;
```

Rows with `NULL` in the tested column are excluded.

## Exercise

Display employees whose `Department` is not `NULL`.