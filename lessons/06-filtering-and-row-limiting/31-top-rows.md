# Lesson 31: Selecting TOP Rows

SQL Server uses `TOP` to limit how many rows a query returns.

## Sample Table

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 200 |
| 102 | 2 | 350 |
| 103 | 1 | 150 |
| 104 | 3 | 500 |
| 105 | 4 | 250 |

## Syntax

```sql
SELECT TOP (number) columns
FROM table_name;
```

## Example

```sql
SELECT TOP (3) *
FROM Orders;
```

Without `ORDER BY`, SQL Server does not guarantee which rows are returned.

## Exercise

Display the first 2 rows from `Orders`.