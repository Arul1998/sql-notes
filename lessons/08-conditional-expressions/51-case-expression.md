# Lesson 51: CASE Expression

The `CASE` expression adds conditional logic to a query.

It checks a condition and returns a value based on whether the condition is true or false.

## Sample Table

Imagine this `Orders` table:

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 200 |
| 102 | 2 | 500 |
| 103 | 1 | 150 |
| 104 | 3 | 750 |
| 105 | 4 | 300 |

## Syntax

```sql
SELECT column_name,
       CASE
           WHEN condition THEN result_if_true
           ELSE result_if_false
       END AS new_column_name
FROM table_name;
```

## Example

```sql
SELECT EmployeeName,
       Salary,
       CASE
           WHEN Salary >= 50000 THEN 'High Salary'
           ELSE 'Standard Salary'
       END AS SalaryLevel
FROM Employees;
```

This creates a calculated column named `SalaryLevel`. It does not change the table data.

## Exercise

Display `OrderId`, `Amount`, and a calculated column named `OrderSize` from the `Orders` table.

- If `Amount` is 500 or more, display `Large`.
- Otherwise, display `Small`.
