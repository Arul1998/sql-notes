# Lesson 10: LIKE

`LIKE` searches for a text pattern.

Imagine this `Employees` table:

| EmployeeName | Department |
|---|---|
| Arul | IT |
| Priya | Finance |
| John | IT |
| Sara | Finance |
| Adam | Sales |

To display names starting with A:

```sql
SELECT EmployeeName
FROM Employees
WHERE EmployeeName LIKE 'A%';
```

Common patterns:

| Pattern | Meaning |
|---|---|
| `'A%'` | Starts with A |
| `'%a'` | Ends with a |
| `'%ar%'` | Contains ar |
| `'A___'` | A followed by exactly three characters |

- `%` represents any number of characters.
- `_` represents exactly one character.

SQL generally follows this pattern:

```sql
SELECT column_name
FROM table_name
WHERE column_name LIKE 'pattern';
```

## Exercise

Display `EmployeeName` and `Department` for employees whose name starts with S.
