# Lesson 148 Answer: QUOTENAME

## Exercise

Using `DatabaseColumns`, display `ColumnId`, `ColumnName`, and `SafeColumnName`. Use `QUOTENAME()` with its default square brackets to enclose each `ColumnName`.

## Sample Table

| ColumnId | ColumnName |
|---:|---|
| 1 | Customer Name |
| 2 | Order Date |
| 3 | Product Price |
| 4 | Employee Salary |

## Answer

```sql
SELECT
    ColumnId,
    ColumnName,
    QUOTENAME(ColumnName) AS SafeColumnName
FROM DatabaseColumns;
```

## Expected Result

| ColumnId | ColumnName | SafeColumnName |
|---:|---|---|
| 1 | Customer Name | `[Customer Name]` |
| 2 | Order Date | `[Order Date]` |
| 3 | Product Price | `[Product Price]` |
| 4 | Employee Salary | `[Employee Salary]` |
