# Lesson 3: Comparison Operators

Comparison operators compare values in a condition.

Imagine this `Employees` table:

| EmployeeId | EmployeeName | Age | Salary |
|---:|---|---:|---:|
| 1 | Arul | 28 | 36000 |
| 2 | Priya | 32 | 45000 |
| 3 | John | 25 | 30000 |
| 4 | Sara | 35 | 52000 |
| 5 | Adam | 29 | 34000 |

Common comparison operators:

| Operator | Meaning |
|---|---|
| `=` | Equal to |
| `<>` | Not equal to |
| `>` | Greater than |
| `<` | Less than |
| `>=` | Greater than or equal to |
| `<=` | Less than or equal to |

To display employees earning more than £35,000:

```sql
SELECT EmployeeName, Salary
FROM Employees
WHERE Salary > 35000;
```

To display employees aged 28 or younger:

```sql
SELECT EmployeeName, Age
FROM Employees
WHERE Age <= 28;
```

SQL generally follows this pattern:

```sql
SELECT column_name
FROM table_name
WHERE column_name comparison_operator value;
```

## Exercise

Write a query that displays `EmployeeName` and `Salary` for employees earning at least £40,000.
