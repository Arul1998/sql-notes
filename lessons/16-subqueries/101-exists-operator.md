# Lesson 101: EXISTS Operator

`EXISTS` checks whether a subquery returns at least one row.

It is useful for finding records that have matching data in another table.

## Sample Tables

**Employees**

| EmployeeId | EmployeeName |
|---:|---|
| 1 | John |
| 2 | Sarah |
| 3 | David |

**Orders**

| OrderId | EmployeeId | Amount |
|---:|---:|---:|
| 101 | 1 | 250 |
| 102 | 1 | 400 |
| 103 | 3 | 150 |

## Syntax

```sql
SELECT columns
FROM table1 AS t1
WHERE EXISTS (
    SELECT 1
    FROM table2 AS t2
    WHERE t2.Id = t1.Id
);
```

## Example

Find employees who have at least one order:

```sql
SELECT EmployeeId, EmployeeName
FROM Employees AS e
WHERE EXISTS (
    SELECT 1
    FROM Orders AS o
    WHERE o.EmployeeId = e.EmployeeId
);
```

`EXISTS` returns true when at least one matching order is found. An employee appears only once even if they have several orders.

## Exercise

Write a query to display `EmployeeId` and `EmployeeName` from `Employees`, but only for employees who have at least one record in `Orders`.

Use `EXISTS`.
