# Lesson 7: DISTINCT

`DISTINCT` removes duplicate values from query results.

Imagine this `Employees` table:

| EmployeeName | Department | Age |
|---|---|---:|
| Arul | IT | 28 |
| Priya | Finance | 32 |
| John | IT | 25 |
| Sara | Finance | 35 |
| Adam | Sales | 29 |

To display each department only once:

```sql
SELECT DISTINCT Department
FROM Employees;
```

The result contains IT, Finance, and Sales without repeating them.

You can also sort distinct values:

```sql
SELECT DISTINCT Department
FROM Employees
ORDER BY Department;
```

SQL generally follows this pattern:

```sql
SELECT DISTINCT column_name
FROM table_name;
```

## Exercise

Write a query that displays the unique employee ages from the `Employees` table, sorted from youngest to oldest.
