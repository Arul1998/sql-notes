# Lesson 47: Finding NULL Values

Use `IS NULL` to find rows where a column has no value.

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
WHERE column_name IS NULL;
```

## Example

```sql
SELECT *
FROM Employees
WHERE Department IS NULL;
```

Do not use `= NULL`; SQL requires `IS NULL`.

## Exercise

Display employees whose `Department` is `NULL`.