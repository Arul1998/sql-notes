# Lesson 29: Deleting All Rows

A `DELETE` statement without a `WHERE` clause removes every row from a table. The table itself still exists.

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
DELETE FROM table_name;
```

## Example

```sql
DELETE FROM Orders;
```

This operation affects every row, so use it carefully.

## Exercise

Delete all rows from the `Employees` table.