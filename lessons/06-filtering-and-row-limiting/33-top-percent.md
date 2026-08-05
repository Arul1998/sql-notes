# Lesson 33: Selecting TOP PERCENT

`TOP PERCENT` returns a percentage of the rows instead of a fixed number.

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
SELECT TOP (percentage) PERCENT columns
FROM table_name;
```

## Example

```sql
SELECT TOP (50) PERCENT *
FROM Employees;
```

SQL Server rounds the calculated number of rows up to the next whole row.

## Exercise

Display the top 25 percent of rows from `Employees`.