# Lesson 148: QUOTENAME

`QUOTENAME()` wraps SQL identifiers in delimiters, using square brackets by default. It escapes closing brackets and accepts at most 128 input characters.

## Sample Table

| ColumnId | ColumnName |
|---:|---|
| 1 | Customer Name |
| 2 | Order Date |
| 3 | Product Price |
| 4 | Employee Salary |

## Syntax

```sql
QUOTENAME(identifier_text)
```

## Example

```sql
SELECT QUOTENAME('Customer Name') AS SafeColumnName;
```

## Exercise

Using `DatabaseColumns`, display `ColumnId`, `ColumnName`, and `SafeColumnName`. Use `QUOTENAME()` with its default square brackets to enclose each `ColumnName`.
